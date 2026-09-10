# Contributing

## Purpose and audience

Contribute useful outdoor-LCD engineering knowledge for system integrators, engineers, technical consultants, distributors, project designers and maintenance technicians. Favor a small number of carefully reviewed resources over frequent generic articles.

## Branch and review process

1. Inspect existing material and preserve useful content and history.
2. Work on a branch such as `docs/...`, `fix/...`, `tool/...`, `research/...` or `setup/...`. Never push normal work directly to `main`.
3. Keep each change focused. Check navigation, terminology, evidence and confidentiality before opening a pull request.
4. Use the [pull request template](.github/PULL_REQUEST_TEMPLATE.md). Explain the purpose, changes, technical verification, risks and specific human decisions.
5. Wait for SUNTUNE human approval. Automated success is never approval to merge your own PR. Do not enable automatic merging or publication of unreviewed engineering content.

Do not delete repositories, change visibility or access permissions, disable security protections, remove branch/ruleset protections, expose secrets, rewrite history or force-push protected branches without explicit human authorization.

CODEOWNERS expresses review ownership; it does not itself enforce approval. Repository protection settings require separate human configuration. Do not assume documented policy is technically enforced.

## Technical integrity

Never fabricate test results, certifications, measurements, customer projects, failure rates, laboratory data, environmental-test results, product specifications, customer names, case studies or performance claims.

Use these labels wherever content mixes evidence types:

| Category | Required support |
| --- | --- |
| **Established engineering principle** | A traceable technical source and an explanation of applicability and limitations |
| **Engineering estimate** | Inputs, units, assumptions, method, uncertainty and limits; identify hypothetical examples |
| **SUNTUNE-verified data** | Authorized evidence with product/configuration, method, conditions, date and verification responsibility |

Mark unverified information `[VERIFICATION REQUIRED]` and explain what evidence is missing. Never relabel estimates as measurements or general principles as SUNTUNE results. Resolve unsupported claims before approval, or remove them from publication. Do not attach confidential evidence to a public PR; use an authorized internal review channel.

For technical documents, record status, author or responsible maintainer, review date, scope, applicable configuration, sources and outstanding verification. Cite sources close to claims with document title, issuer, revision/date and relevant section or URL. Do not copy protected standards or proprietary documents into the repository.

## Writing and document structure

Prefer: **why something happens → how to diagnose it → engineering trade-offs → practical mitigation**.

Use clear English, descriptive filenames, consistent terminology, explicit units and relative links for repository navigation. Define abbreviations on first use. Explain boundary conditions and uncertainty rather than implying universal performance.

A technical article should normally include:

- Scope, audience, status and review date.
- Mechanism or engineering principle.
- Diagnostic observations and evidence needed.
- Options, trade-offs and practical mitigation.
- Limits, verification requirements and references.

Avoid unsupported promotional terms such as "best", "world-class", "industry-leading", "revolutionary", "perfect" and "guaranteed". Never imply a symptom establishes a unique root cause without evidence.

## Confidentiality before submission

Never publish customer-confidential information, unauthorized customer names, supplier-sensitive information, internal pricing, passwords or API credentials, proprietary drawings, confidential BOM information, private contact information or unreleased commercial information.

Flag uncertain material for human review before placing it in this public repository, including branches, PRs, issues, attachments and logs. Remove identifying details from proposed field notes and obtain permission for remaining content. If a credential is exposed, alert the authorized maintainer through a private channel without repeating it publicly.

## Tools and automation

Tools must document formulas, input units, assumptions, boundaries, dependencies and meaningful validation examples. Identify estimates explicitly and avoid unsupported product recommendations.

The [automation plan](.github/workflows/README.md) describes future checks. Checks assist review; they cannot certify engineering accuracy, confidentiality or publication authorization.

## Licensing and pilot review

The licensing decision is pending in [LICENSE](LICENSE). Do not add third-party material without confirming permission and attribution requirements.

At the end of the 30-day pilot, humans should assess technical usefulness, evidence quality, reviewer effort and maintainability before expanding the library. There is no daily publishing requirement.
