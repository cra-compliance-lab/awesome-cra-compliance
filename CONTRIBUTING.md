# Contributing to Awesome CRA Compliance

Thank you for wanting to contribute! This list aims to be the definitive community resource for the EU Cyber Resilience Act.

## What belongs here

- **Official EU texts**: regulation, delegated acts, implementing acts, Commission guidance, FAQ.
- **Harmonised standards** (both under M/606 and reference standards cited by Commission guidance).
- **EU project outputs** from the CRA Cluster (CYBERSTAND, STAN4CRA, SECURE, OCCTET, CONFIRMATE, CURIUM, etc.).
- **ENISA / BSI / national-authority publications** related to CRA.
- **Webinars, conference talks, podcasts** with publicly available recordings.
- **Books and academic research** directly relevant to CRA compliance, threat modelling, vulnerability management, SBOM, or conformity assessment.
- **Open-source tools and frameworks** that materially help with CRA obligations.

## What does NOT belong here

- Proprietary / paywalled vendor marketing material.
- Blog posts without substantive content.
- Duplicate entries.
- Personal opinions presented as fact.
- **Links to copyrighted PDFs hosted anywhere other than the rights-holder.**

## How to submit

1. Fork this repository.
2. Add your entry to the correct section, in alphabetical order where the section uses one.
3. Use the entry format below.
4. Open a pull request with a clear title (e.g., `add EN 304-624 PKI deep-dive slides`) and explain in the description why the resource belongs on the list.

## Entry format

```
- [Title](URL) - One-to-two factual sentences about what the resource is and how it relates to the CRA. *Paid/free/draft.*
```

Rules:

- **URL** must point to the official source (publisher page, regulator page, project site, standards catalogue). **Do not link to uploaded PDFs hosted on third-party sites.**
- **Title** must match the resource's actual title.
- **Description** is factual, not promotional. State scope and CRA relevance. Two sentences maximum.
- **Annotations** (`*Paid standard.*`, `*Free download.*`, `*Draft.*`) help readers know what to expect.

## Copyright

- **Standards** (ISO, IEC, EN, ETSI, IEEE, BSI copyrighted):
  - Link to the official catalogue page.
  - Do not upload PDFs.
  - Describe scope factually (fair use).
- **Books**:
  - Link to publisher or a neutral reference page (Google Books, WorldCat).
  - Do not upload PDFs or excerpts.
  - Provide a 1–2 sentence editorial summary.
- **Official EU publications**:
  - Link to [EUR-Lex](https://eur-lex.europa.eu/) or the Commission DG CNECT page.
  - PDFs in this repo's `docs/eu/` are mirrored under the Commission's reuse policy ([Decision 2011/833/EU](https://eur-lex.europa.eu/eli/dec/2011/833/oj)); always include the source URL too.
- **ESO/ETSI webinar slides**:
  - Slides released by CEN, CENELEC, ETSI, ENISA, and the STAN4CRA/CYBERSTAND projects have been publicly distributed. They can be mirrored here. Always link to the authoritative upstream location as well (YouTube, project website).

## Style

- Sentence case for section headings (`## Standards & Standardisation`, not `## Standards And Standardisation`).
- Markdown bullets with `-`, not `*`.
- One space after the bullet, no trailing whitespace.
- Descriptions end with a full stop.
- Use Oxford spelling (organisation, standardisation).

## Review

Pull requests are reviewed for:

1. Accuracy (does the link work? is the description factual?).
2. Relevance (does it clearly help a CRA practitioner?).
3. Copyright compliance.
4. Formatting consistency.

Maintainers may request edits before merging.

## Code of conduct

Be respectful. Assume good faith. Disagreements about inclusion are normal — discuss in the PR and escalate to a maintainer if you cannot agree.
