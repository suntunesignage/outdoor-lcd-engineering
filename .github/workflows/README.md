# Automation preparation

This directory reserves the location for future GitHub Actions workflows.
There are no executable workflows in this foundation change, and no automated
checks are currently provided by these files.

## Planned checks

| Check | Intended behavior |
| --- | --- |
| Markdown validation | Check document structure and formatting with a reviewed configuration |
| Broken-link checking | Check local paths first; report external failures with retries and human assessment |
| Spelling and terminology | Use a reviewed dictionary for LCD terminology, abbreviations and product names |
| Accidental secret detection | Flag potential credentials without printing secret values in public logs |
| Repository structure | Check required files, navigation and expected content locations |

## Implementation requirements

Introduce checks in a focused, human-reviewed PR. Use pull-request events and
manual execution where appropriate. Default to `permissions: contents: read`
and grant no write permissions unless separately justified and authorized.

Pin external actions to reviewed full commit SHAs, pin dependencies, set timeouts
and avoid persisting checkout credentials. Treat contributor content as
untrusted. Do not run untrusted PR code with secrets, elevated tokens or
`pull_request_target`. Do not expose sensitive findings in logs.

Do not create automatic publishing, merging, generated-article commits or
unreviewed content updates. Test check behavior with representative valid and
invalid examples before proposing that a human make a check required.

Automated checks cannot verify engineering truth or authorization. Required
reviews and branch protections are repository settings, not supplied by this
directory or CODEOWNERS.
