# Awesome CRA Compliance [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of resources for the EU **Cyber Resilience Act** — Regulation (EU) 2024/2847 — covering the regulation itself, harmonised standards, conformity assessment, vulnerability handling, sector-specific guidance, research, tools, and community projects.

[![License: CC0-1.0](https://img.shields.io/badge/License-CC0%201.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

The CRA is the first EU-wide horizontal regulation setting mandatory cybersecurity requirements for all hardware and software products with digital elements placed on the Union market. It entered into force on **10 December 2024**, its vulnerability-reporting duties start **11 September 2026**, and its full requirements apply from **11 December 2027**. This list gathers the most useful public resources for engineers, assessors, lawyers, and managers working on CRA compliance.

> **Disclaimer**: This list curates and describes publicly available resources related to the EU Cyber Resilience Act. Copyrighted materials (ISO/IEC, ETSI, BSI, IEEE standards, and published books) are linked to their **official catalogue pages only** — no copyrighted content is hosted in this repository. The PDFs stored in `presentations/` and `docs/eu/` are either (a) official EU publications published under the Commission's reuse policy (Decision 2011/833/EU), or (b) webinar slide decks released publicly by CEN, CENELEC, ETSI, ENISA, or other EU projects. All descriptions are factual summaries for informational purposes.

---

## Contents

- [The Cyber Resilience Act](#the-cyber-resilience-act)
  - [Official Regulation & Legislation](#official-regulation--legislation)
  - [Commission Guidance & FAQ](#commission-guidance--faq)
  - [Delegated & Implementing Acts](#delegated--implementing-acts)
  - [Timeline & Milestones](#timeline--milestones)
- [Standards & Standardisation](#standards--standardisation)
  - [M/606 Standardisation Request](#m606-standardisation-request)
  - [Horizontal Standards (CEN/CLC JTC 13)](#horizontal-standards-cenclc-jtc-13)
  - [Vertical Standards (ETSI EN 304-6xx series)](#vertical-standards-etsi-en-304-6xx-series)
  - [Reference Standards (ISO/IEC, IEC 62443, BSI TR-03183)](#reference-standards-isoiec-iec-62443-bsi-tr-03183)
- [Conformity Assessment & Certification](#conformity-assessment--certification)
  - [EUCC (Common Criteria)](#eucc-common-criteria)
  - [Conformity Assessment Procedures (Modules A, B+C, H)](#conformity-assessment-procedures-modules-a-bc-h)
- [Vulnerability Handling & Reporting](#vulnerability-handling--reporting)
  - [SBOM & Transparency](#sbom--transparency)
  - [Coordinated Vulnerability Disclosure](#coordinated-vulnerability-disclosure)
  - [ENISA Guidelines](#enisa-guidelines)
- [Product-Category Deep Dives (Webinars & Slides)](#product-category-deep-dives-webinars--slides)
  - [CEN-CENELEC Horizontal Webinars](#cen-cenelec-horizontal-webinars)
  - [ETSI Vertical-Standard Deep Dives (STAN4CRA)](#etsi-vertical-standard-deep-dives-stan4cra)
  - [Q&A and Workshop Reports](#qa-and-workshop-reports)
- [Relationship to Other EU Regulation](#relationship-to-other-eu-regulation)
- [EU CRA Cluster Projects](#eu-cra-cluster-projects)
- [Books & Long-Form References](#books--long-form-references)
- [Academic & Research](#academic--research)
- [Community, Portals & Further Reading](#community-portals--further-reading)
- [Contributing](#contributing)
- [License](#license)
- [Maintainer](#maintainer)

---

## The Cyber Resilience Act

### Official Regulation & Legislation

The authoritative sources. Always read these before secondary material.

- [Regulation (EU) 2024/2847 — Cyber Resilience Act](https://eur-lex.europa.eu/eli/reg/2024/2847/oj) — The full legal text: 71 articles, 8 annexes. *Essential reading.* Local copy: [`docs/eu/cra-regulation-2024-2847.pdf`](docs/eu/cra-regulation-2024-2847.pdf).
- [Commission Implementing Regulation on important and critical products](https://eur-lex.europa.eu/eli/reg_impl/2025/2392/oj/eng) — Clarifies which product classes fall under Annex III (important, Class I/II) and Annex IV (critical). Local copy: [`docs/eu/important-and-critical-products-regulation.pdf`](docs/eu/important-and-critical-products-regulation.pdf).
- [CRA Impact Assessment (European Commission, 2022)](https://digital-strategy.ec.europa.eu/en/library/cyber-resilience-act-impact-assessment) — The Commission's 4-part impact assessment (main report, annexes, Part 3, summary). Useful for understanding policy rationale behind each obligation.

### Commission Guidance & FAQ

Non-binding but highly influential. Notified bodies and market-surveillance authorities will reference these.

- [Commission Guidance on the application of Regulation (EU) 2024/2847](https://ec.europa.eu/info/law/better-regulation/have-your-say/initiatives/16959-Draft-Commission-guidance-on-the-Cyber-Resilience-Act_en) — The Commission's official application guidance. Explains scope (Art. 2), product categories (Art. 7-8), manufacturer obligations (Art. 13), and conformity routes (Art. 32). Local copy: [`docs/eu/commission-guidance-on-cra-application.pdf`](docs/eu/commission-guidance-on-cra-application.pdf).
- [CRA FAQ (European Commission)](https://digital-strategy.ec.europa.eu/en/library/cyber-resilience-act-implementation-frequently-asked-questions) — Quick answers on scope, definitions, timelines, and common manufacturer questions. Local copy: [`docs/eu/cra-faq.pdf`](docs/eu/cra-faq.pdf).
- [CRA Requirements → Standards Mapping](https://www.enisa.europa.eu/publications/cyber-resilience-act-requirements-standards-mapping) — The Commission's official mapping of every CRA essential requirement to its intended harmonised standard. Local copy: [`docs/eu/cra-requirements-to-standards-mapping.pdf`](docs/eu/cra-requirements-to-standards-mapping.pdf).
- [EU Supply-Chain Toolbox](https://digital-strategy.ec.europa.eu/en/library/toolbox-improve-ict-supply-chain-security) — Commission guidance on supply-chain security due diligence, informs Art. 13(11) and Annex I Part II (1) SBOM. Local copy: [`docs/eu/eu-supply-chain-toolbox.pdf`](docs/eu/eu-supply-chain-toolbox.pdf).

### Delegated & Implementing Acts

- [Standardisation Request M/606](https://ec.europa.eu/growth/tools-databases/enorm/mandate/606_en) — The formal mandate to CEN, CENELEC, and ETSI to produce harmonised standards supporting the CRA. Local copy: [`docs/eu/M606-standardisation-request-work-programme.pdf`](docs/eu/M606-standardisation-request-work-programme.pdf).
- [Delegated Act repealing RED cybersecurity requirements (C(2026) 778)](https://ec.europa.eu/transparency/documents-register/detail?ref=C(2026)778&lang=en) — Transitional measure removing overlap between RED (2014/53/EU) Art. 3(3)(d-f) and CRA from 11 December 2027. Local copy: [`docs/eu/red-delegated-act-repeal.pdf`](docs/eu/red-delegated-act-repeal.pdf).

### Timeline & Milestones

| Date | Milestone |
|---|---|
| 10 December 2024 | CRA entered into force |
| 11 June 2026 | Notifying authorities designate notified bodies (Art. 35 onwards) |
| 11 September 2026 | Reporting obligations apply (Art. 14: actively exploited vulnerabilities, severe incidents) |
| 11 December 2027 | All other obligations apply — full CE marking requirement |
| Until 11 December 2027 | Existing RED cybersecurity regime (Delegated Regulation 2022/30) remains valid for in-scope radio equipment |

---

## Standards & Standardisation

### M/606 Standardisation Request

The M/606 mandate defines **40+ harmonised standards** — 4 horizontal (applicable to all products) and 36+ vertical (per product category). Compliance with a harmonised standard creates a presumption of conformity with the CRA essential requirements it covers (Art. 27).

- [STAN4CRA Portal](https://www.stan4cra.eu) — The official tracking portal where CEN, CENELEC, and ETSI publish development progress of every CRA harmonised standard. *Bookmark this.*
- [CYBERSTAND Project](https://cyberstand.eu) — EU-funded initiative onboarding 200+ experts to contribute to CRA standards; tracks expert participation and working-group outputs.

### Horizontal Standards (CEN/CLC JTC 13)

The `prEN 40000-1-x` family covers requirements that apply across all CRA products. Drafts are currently under public enquiry; final versions will be cited in the Official Journal.

- [prEN 40000-1-1:2026-03 — General principles and common requirements](https://www.dinmedia.de/en/draft-standard/din-en-40000-1-1/399664868) - Scope, definitions, compliance framework for CRA. *Currently draft under CEN-CLC JTC 13.*
- [prEN 40000-1-2:2026-03 — Cybersecurity requirements (Annex I Part I Point 1)](https://www.dinmedia.de/en/draft-standard/din-en-40000-1-2/399705978) - Covers the catch-all "no known exploitable vulnerabilities" obligation and security-by-design requirements. *Paid once published; free during public enquiry.*
- [prEN 40000-1-3:2026-02 — Vulnerability handling (Annex I Part II)](https://www.dinmedia.de/en/draft-standard/din-en-40000-1-3/398007938) - Operational requirements for vulnerability management, SBOM, coordinated disclosure, security updates. *Draft; see WG-9 PT3 workshop materials.*
- [prEN 40000-1-4 — Security controls (Annex I Part I Point 2)](https://standards.cencenelec.eu/) - The 13-point security-controls catalogue implementing Annex I Part I (2)(a)–(m).

### Vertical Standards (ETSI EN 304-6xx series)

Per-product-category standards under ETSI TC CYBER. These map to **Annex III (Important products)** classes. Final versions will be published at no cost via the [ETSI standards portal](https://www.etsi.org/standards).

> 📥 **Current drafts are publicly downloadable** from the ETSI docbox at **<https://docbox.etsi.org/CYBER/EUSR/Open>** — this is the authoritative source for the latest working versions of every EN 304-6xx standard while they are under public enquiry.

- [EN 304-617 — Browsers](https://www.etsi.org/deliver/etsi_en/304600_304699/304617/) - Cybersecurity requirements for standalone and embedded browsers. *Class I Important product. Free draft.*
- [EN 304-618 — Password Managers](https://www.etsi.org/deliver/etsi_en/304600_304699/304618/) - Requirements for password manager products; covers credential storage, master-password handling, browser-integration threats. *Class I Important product.*
- [EN 304-619 — Antivirus / Antimalware](https://www.etsi.org/deliver/etsi_en/304600_304699/304619/) - Cybersecurity requirements for software that searches for, removes, or quarantines malicious software. *Class I Important product.*
- [EN 304-620 — VPN Products](https://www.etsi.org/deliver/etsi_en/304600_304699/304620/) - Requirements for products with the function of virtual private network. *Class I Important product.*
- [EN 304-622 — SIEM Systems](https://www.etsi.org/deliver/etsi_en/304600_304699/304622/) - Security information and event management system requirements. *Class I Important product.*
- [EN 304-623 — Boot Managers](https://www.etsi.org/deliver/etsi_en/304600_304699/304623/) - Requirements for boot managers including UEFI firmware and multi-stage boot loaders. *Class I Important product.*
- [EN 304-624 — PKI & Digital Certificate Issuance Software](https://www.etsi.org/deliver/etsi_en/304600_304699/304624/) - Public-key infrastructure and certificate issuance software. *Class I Important product.*
- [EN 304-625 — Physical & Virtual Network Interfaces](https://www.etsi.org/deliver/etsi_en/304600_304699/304625/) - Cybersecurity for physical and virtual network interface products. *Class I Important product.*
- [EN 304-626 — Operating Systems](https://www.etsi.org/deliver/etsi_en/304600_304699/304626/) - CRA requirements for operating systems. *Class I Important product.*
- [EN 304-627 — Routers, Modems and Switches](https://www.etsi.org/deliver/etsi_en/304600_304699/304627/) - Covers internet-facing routers, modems, and switches. *Class I Important product.*
- [EN 304-631 — Smart Home Virtual Assistants](https://www.etsi.org/deliver/etsi_en/304600_304699/304631/) - Requirements for voice assistants and smart-home hubs.
- [EN 304-632 — Smart Home Security Products](https://www.etsi.org/deliver/etsi_en/304600_304699/304632/) - Cameras, smart locks, alarm devices.
- [EN 304-633 — Connected Toys](https://www.etsi.org/deliver/etsi_en/304600_304699/304633/) - Children's products with digital elements (Annex III item 18; Recital 10).
- [EN 304-634 — Personal Wearables](https://www.etsi.org/deliver/etsi_en/304600_304699/304634/) - Smartwatches, fitness trackers, other wearables.
- [EN 304-635 — Virtualisation and Containers](https://www.etsi.org/deliver/etsi_en/304600_304699/304635/) - Requirements for hypervisors and container runtimes.
- [EN 304-636 — Firewalls, IDS/IPS](https://www.etsi.org/deliver/etsi_en/304600_304699/304636/) - Class II Important-product standard.

### Reference Standards (ISO/IEC, IEC 62443, BSI TR-03183)

These standards are widely referenced by CRA guidance but are **not** the harmonised standards themselves. They provide methodology and good practice. All are **copyrighted** — purchase from the official catalogue.

- [IEC 62443-4-1 — Secure product development lifecycle](https://webstore.iec.ch/publication/33615) - Process requirements for developing secure industrial products. Often cited as the operational backbone for Annex I Part I (1) security-by-design. *Paid standard.*
- [IEC 62443-4-2 — Technical security requirements for IACS components](https://webstore.iec.ch/publication/34421) - Component-level security requirements for industrial control products; informs prEN 40000-1-4 security controls. *Paid standard.*
- [ISO/IEC 27005:2022 — Information security risk management](https://www.iso.org/standard/80585.html) - Methodology for information-security risk assessment referenced by Art. 13(2) risk-assessment obligation. *Paid standard.*
- [ISO/IEC 29147:2018 — Vulnerability disclosure](https://www.iso.org/standard/72311.html) - Framework for handling external vulnerability reports; CRA Annex I Part II (5) CVD reference. *Paid standard.*
- [ISO/IEC 30111:2019 — Vulnerability handling processes](https://www.iso.org/standard/69725.html) - Internal vulnerability-handling process requirements; paired with 29147 for full CVD lifecycle. *Paid standard.*
- [ISO/IEC 27036-3:2023 — Supply-chain ICT security](https://www.iso.org/standard/78906.html) - Information security for ICT supplier relationships; maps to Art. 13(11) third-party diligence. *Paid standard.*
- [ISO/IEC TR 5895:2022 — Vulnerability disclosure guidance](https://www.iso.org/standard/81981.html) - Explanatory companion to 29147/30111. *Paid standard.*
- [ISO/IEC 27001:2022 — Information security management](https://www.iso.org/standard/27001) - Organisation-level ISMS; referenced by CRA conformity assessment for manufacturer quality processes. *Paid standard.*
- [ETSI TS 102 165-1 — Threat, vulnerability, risk analysis (TVRA)](https://www.etsi.org/deliver/etsi_ts/102100_102199/10216501/) - ETSI methodology for security analysis of communication systems. *Free download from ETSI.*
- [BSI TR-03183-1 — Cyber Resilience Requirements for Manufacturers and Products](https://www.bsi.bund.de/EN/Themen/Unternehmen-und-Organisationen/Standards-und-Zertifizierung/Technische-Richtlinien/TR-nach-Thema-sortiert/tr03183/TR-03183_node.html) - German Federal Office for Information Security's technical guideline — Part 1: general requirements; structured companion to CRA Annex I. *Free download.*
- [BSI TR-03183-2 — Software Bill of Materials (SBOM)](https://www.bsi.bund.de/EN/Themen/Unternehmen-und-Organisationen/Standards-und-Zertifizierung/Technische-Richtlinien/TR-nach-Thema-sortiert/tr03183/TR-03183_node.html) - Part 2: SBOM requirements and formats. *Free download; authoritative for Annex I Part II (1).*
- [BSI TR-03183-3 — Vulnerability Disclosure & Reporting](https://www.bsi.bund.de/EN/Themen/Unternehmen-und-Organisationen/Standards-und-Zertifizierung/Technische-Richtlinien/TR-nach-Thema-sortiert/tr03183/TR-03183_node.html) - Part 3: vulnerability reporting; directly maps to CRA Art. 14 and Annex I Part II. *Free download.*

---

## Conformity Assessment & Certification

### EUCC (Common Criteria)

For critical products (Annex IV: HSMs, smart-meter gateways, smartcards) and optionally for important products, EUCC certification at "substantial" assurance level provides a presumption of conformity with CRA essential requirements (Art. 27(8)-(9)).

- [Regulation (EU) 2024/482 — EUCC Scheme](https://eur-lex.europa.eu/eli/reg_impl/2024/482/oj) - The implementing regulation establishing the EUCC scheme under the Cybersecurity Act.
- [ENISA — CRA Implementation via EUCC (Jan 2025)](https://certification.enisa.europa.eu/publications/cyber-resilience-act-implementation-eucc-and-its-applicable-technical-elements_en) - ENISA's authoritative 128-page report mapping EUCC (TOE, SFRs, SARs, Protection Profiles, ITSEFs, CABs) to CRA Annex I requirements. *Essential for any manufacturer choosing EUCC as the CRA conformity route.* Local copy: [`docs/eu/enisa-cra-implementation-via-eucc.pdf`](docs/eu/enisa-cra-implementation-via-eucc.pdf).
- [ENISA — [ANNEX] CRA Implementation via EUCC — Detailed Mapping Tables](https://certification.enisa.europa.eu/publications/cyber-resilience-act-implementation-eucc-and-its-applicable-technical-elements_en) - Companion annex with row-by-row mapping of each Annex I requirement to specific SFRs/SARs. Local copy: [`docs/eu/enisa-cra-implementation-via-eucc-annex-mapping-tables.pdf`](docs/eu/enisa-cra-implementation-via-eucc-annex-mapping-tables.pdf).
- [ENISA — EUCC Vulnerability Management Guidelines v1.1](https://certification.enisa.europa.eu/publications/eucc-guidelines-vulnerability-management-and-disclosure-and-eccg-opinion_en) - How EUCC-certified products must handle vulnerability management during the certification-maintenance period. Local copy: [`docs/eu/enisa-eucc-vulnerability-management-guidelines-v1.1.pdf`](docs/eu/enisa-eucc-vulnerability-management-guidelines-v1.1.pdf).
- [ISO/IEC 15408 (Common Criteria)](https://www.iso.org/standard/72891.html) - The international standard underlying EUCC. *Paid standard.*
- [ISO/IEC 18045 (CEM — Common Evaluation Methodology)](https://www.iso.org/standard/72889.html) - How evaluators actually test CC Targets of Evaluation. *Paid standard.*

### Conformity Assessment Procedures (Modules A, B+C, H)

- [Commission Blue Guide on the implementation of product rules](https://single-market-economy.ec.europa.eu/news/blue-guide-implementation-product-rules-2022-published-2022-06-29_en) - Reference document explaining Module A (self-assessment), Module B+C (EU-type examination), Module H (full quality assurance) as used under the CRA.
- [Module H under the CRA — Eurosmart](https://www.eurosmart.com/cyberact-conference-why-full-quality-assurance-module-h-is-a-strategic-path-to-cra-compliance/) - Industry briefing on full quality-assurance route. Local copy: [`docs/eu/Module H under the Cyber Resilience Act Eurosmart.pdf`](docs/eu/Module%20H%20under%20the%20Cyber%20Resilience%20Act%20Eurosmart.pdf) (if you added it).
- [NANDO database — notified bodies](https://webgate.ec.europa.eu/single-market-compliance-space/notified-bodies) - EU's registry of notified bodies. As notified bodies for the CRA are designated (from 11 June 2026), they will appear in NANDO.

---

## Vulnerability Handling & Reporting

### SBOM & Transparency

CRA Annex I Part II (1) obliges manufacturers to identify and document the components and vulnerabilities in their products, including through a software bill of materials. The draft horizontal harmonised standard **prEN 40000-1-3** (CEN/CLC JTC 13) gives that obligation operational shape through normative requirements in clauses 5.3.8 (software) and 5.3.9 (hardware); for authoritative wording, consult the published draft from your national standards body.

| ID | What the requirement covers (paraphrased) |
|----|-------------------------------------------|
| `[PRE-7-RQ-01]` | Every software component in the product must be inventoried and documented. |
| `[PRE-7-RQ-03]` | Direct dependencies are mandatory; indirect (transitive) dependencies are recommended. |
| `[PRE-7-RQ-04]` | The SBOM has to be machine-readable; SPDX and CycloneDX are the formats explicitly named. |
| `[PRE-7-RQ-06]` | SBOM metadata must include author, version, and ISO-8601 timestamp. |
| `[PRE-7-RQ-07]` | Each component requires a unique identifier — PURL, CPE, and SWHID are given as examples. |
| `[PRE-7-RQ-07-RE]` | Where an upstream vendor supplies a component hash, it must be carried through into the SBOM. |
| `[PRE-8-RQ-02]` | Hardware must also be inventoried: producer, component name, identifier, and firmware version where applicable. |
| `[RLS-2-RQ-03-RE]` | After a vulnerability is fixed, the disclosure must be issued in a machine-readable advisory format; CSAF v2.0 (ISO/IEC 20153:2025) is the named reference. |

> *Summaries paraphrased from the public draft of prEN 40000-1-3 (© CEN-CENELEC); editorial commentary only.*

*Specifications and reference publications:*

- [CISA SBOM landing page](https://www.cisa.gov/sbom) - US CISA hub of SBOM resources; aligns with the CRA approach and is referenced across EU material. *Free.*
- [CSAF v2.0 (OASIS)](https://csaf.io/) - Machine-readable vulnerability advisory format named by prEN 40000-1-3 `[RLS-2-RQ-03-RE]`, published as ISO/IEC 20153:2025. *Free and open.*
- [CycloneDX Specification](https://cyclonedx.org/specification/overview/) - OWASP-maintained SBOM format satisfying prEN 40000-1-3 `[PRE-7-RQ-04]`. *Free and open; current version 1.6.*
- [ENISA — CRA SBOM Study (Nov 2025)](https://www.enisa.europa.eu/news/call-for-feedback-advancing-software-supply-chain-security-together) - ENISA's study on SBOM tooling, formats, and maturity for CRA compliance. *Free; essential reference.*
- [ENISA — SBOM Analysis: Towards an Implementation Guide](https://www.enisa.europa.eu/publications/sbom-analysis) - ENISA guide covering minimum elements, naming conventions, quality criteria, and CI/CD integration. *Free download.*
- [NTIA — The Minimum Elements For a Software Bill of Materials](https://www.ntia.doc.gov/report/2021/minimum-elements-software-bill-materials-sbom) - US baseline of seven SBOM data fields, widely implemented by tooling and aligned with BSI TR-03183-2. *Free.*
- [SPDX Specification](https://spdx.dev/specifications/) - Alternative ISO/IEC 5962:2021 SBOM format, equally accepted under prEN 40000-1-3 `[PRE-7-RQ-04]`. *Free and open.*

*Generation tools (open source):*

- [cdxgen](https://github.com/CycloneDX/cdxgen) - Fast multi-language CycloneDX SBOM generator with monorepo and reachability support. *Apache-2.0.*
- [CycloneDX build plugins](https://github.com/CycloneDX) - Native build-time SBOM generators for Maven, Gradle, npm, Python, .NET, Go, Rust, and PHP. *Open-source; highest-fidelity Build SBOMs per BSI TR-03183-2.*
- [Microsoft sbom-tool](https://github.com/microsoft/sbom-tool) - Enterprise SPDX 2.2 / 3.0 generator using Microsoft Component Detection libraries. *MIT.*
- [OSS Review Toolkit (ORT)](https://github.com/oss-review-toolkit/ort) - End-to-end analyse-scan-report pipeline for SBOM and licence compliance, used across automotive and telecom. *Apache-2.0.*
- [Syft](https://github.com/anchore/syft) - Multi-ecosystem SBOM generator for source, containers, and filesystems, outputting SPDX and CycloneDX. *Apache-2.0.*
- [Tern](https://github.com/tern-tools/tern) - Deep container-layer analyser for Dockerfile-based images, hosted by the Linux Foundation. *BSD-2-Clause.*
- [Trivy](https://github.com/aquasecurity/trivy) - Container and filesystem SBOM generator combined with a vulnerability scanner in one binary. *Apache-2.0.*
- [Yocto Project SPDX generation](https://docs.yoctoproject.org/dev/dev-manual/sbom.html) - Native SPDX SBOM output for embedded and IoT builds using the Yocto/OpenEmbedded framework. *Open-source.*
- [CRANE](https://github.com/cra-norm-engine/crane) - Open-source CRA compliance evidence engine that evaluates SBOMs and related artefacts against machine-readable CRA requirements and produces structured compliance evidence. *AGPL-3.0.*
  
*Validation and quality scoring:*

- [bomber](https://github.com/devops-kung-fu/bomber) - SBOM vulnerability scanner with pluggable data-provider backends. *Apache-2.0.*
- [cra-sbom-evidence](https://github.com/plusultra-tools/cra-sbom-evidence) - CRA Annex I Part II (1) preflight: scores a CycloneDX/SPDX SBOM against BSI TR-03183-2 mandatory fields and emits an Article 14 evidence bundle. *MIT.*
- [CycloneDX CLI](https://github.com/CycloneDX/cyclonedx-cli) - Schema validation, format conversion, and SBOM merge/diff operations. *Apache-2.0.*
- [ntia-conformance-checker](https://github.com/spdx/ntia-conformance-checker) - Automated NTIA Minimum Elements verification for SPDX SBOMs. *Apache-2.0.*
- [sbomqs](https://github.com/interlynk-io/sbomqs) - Quality and compliance scorer with built-in profiles for BSI TR-03183-2, NTIA Minimum Elements, FSCT v3, and OpenChain Telco. *Apache-2.0.*
- [sbom-tools](https://github.com/sbom-tool/sbom-tools) - Semantic SBOM/CBOM diff and scoring tool with CRA, NTIA, and NIST SSDF profiles plus VEX state tracking. *MIT.*
- [SPDX Tools](https://github.com/spdx/tools) - Reference SPDX validator, converter, and model toolkit. *Apache-2.0.*

*Vulnerability analysis and disclosure:*

- [Cosign (sigstore)](https://github.com/sigstore/cosign) - Signs and attests SBOMs and attaches them to OCI artifacts for supply-chain integrity. *Apache-2.0.*
- [Dependency-Track (OWASP)](https://github.com/DependencyTrack/dependency-track) - Continuous SBOM-based component analysis platform with policy engine and VEX support. *Apache-2.0.*
- [Grype](https://github.com/anchore/grype) - CVE scanner that consumes CycloneDX and SPDX SBOMs. *Apache-2.0.*
- [Secvisogram](https://github.com/secvisogram/secvisogram) - CSAF v2.0 advisory editor mapping to prEN 40000-1-3 `[RLS-2-RQ-03-RE]`; maintained with BSI involvement. *MIT.*

*Firmware and binary analysis (IoT / embedded):*

- [Binwalk](https://github.com/ReFirmLabs/binwalk) - Firmware extraction and filesystem-layer analysis tool. *MIT.*
- [EMBA](https://github.com/e-m-b-a/emba) - Automated embedded-firmware security analyser with component identification and CVE matching. *GPL-3.0.*
- [FACT (Fraunhofer FKIE)](https://github.com/fkie-cad/FACT_core) - Firmware Analysis and Comparison Tool used by BSI and European CERTs. *GPL-3.0.*
- [ScanCode Toolkit (nexB)](https://github.com/nexB/scancode-toolkit) - Licence and origin detection for binary and source trees. *Apache-2.0.*

*Commercial SCA / SBOM platforms:*

- [Black Duck (Synopsys)](https://www.synopsys.com/software-integrity.html) - Binary-code fingerprinting and snippet detection, common in automotive and medical compliance programmes. *Commercial.*
- [FOSSA](https://fossa.com/) - Software composition analysis combining licence compliance with SBOM generation. *Commercial.*
- [Insignary Clarity](https://www.insignary.com/) - Binary-level fingerprinting without source-code access. *Commercial.*
- [Mend](https://www.mend.io/) - Binary hash matching, policy engine, and vulnerability management. *Commercial.*
- [Snyk](https://snyk.io/) - Developer-centric SCA with SBOM export and vulnerability detection. *Commercial.*

### Coordinated Vulnerability Disclosure

- [ENISA — Good practice guide on vulnerability disclosure](https://www.enisa.europa.eu/publications/vulnerability-disclosure) - ENISA's multi-stakeholder guide, often cited by Art. 13(8) and Annex I Part II (5). *Free download.*
- [FIRST — PSIRT Services Framework](https://www.first.org/standards/frameworks/psirts/) - Framework for operating a Product Security Incident Response Team; critical for CRA vulnerability-handling obligations. *Free.*
- [OASIS CSAF (Common Security Advisory Framework)](https://csaf.io/) - Machine-readable security advisory format used by Siemens, Red Hat, Cisco and others for CVD automation. *Free and open.*
- **ENISA — Single Reporting Platform** *(not yet released — placeholder)* - Art. 14 requires early warning, incident, and vulnerability reports to be routed through a single reporting platform run by ENISA. ENISA has not yet published the platform or its technical interface; monitor [ENISA announcements](https://www.enisa.europa.eu/news) for release news.

### ENISA Guidelines

- [ENISA](https://www.enisa.europa.eu/) - The EU Agency for Cybersecurity. Operates the CSIRTs Network, coordinates CRA reporting, runs the EUCC scheme, and publishes technical guidance. *Primary institutional source.*
- [EU CSIRT Network](https://csirtsnetwork.eu/) - Coordinated incident response across member states; designated CSIRTs are recipients of Art. 14 reports.

---

## Product-Category Deep Dives (Webinars & Slides)

The following webinars were produced by the European Standardisation Organisations (CEN, CENELEC, ETSI) and the STAN4CRA project. Slide decks are public; YouTube recordings are linked directly. All PDFs are mirrored locally in `presentations/`.

### CEN-CENELEC Horizontal Webinars

- [Webinar: Standards Supporting the Cyber Resilience Act](https://www.youtube.com/watch?v=KVr9zSZ0nUU) (CEN-CENELEC, 10 Mar 2025) - Overview of the CRA standardisation landscape covering horizontal and vertical standards under M/606. Good entry point. Slides: [`presentations/2025-03-10_webinar_cyberresilience_act.pdf`](presentations/2025-03-10_webinar_cyberresilience_act.pdf).
- [CRA Workshop: Deep Dive on Vulnerability Handling](https://www.youtube.com/watch?v=o5bgzF8riRw) (CEN-CENELEC-ETSI, 22 Jul 2025) - Deep dive on Annex I Part II and prEN 40000-1-3 covering SBOM, CVD, security updates. Slides: [`presentations/cen-clc-jtc-13-wg-9_pt3_cra_workshop_2025-07-22.pdf`](presentations/cen-clc-jtc-13-wg-9_pt3_cra_workshop_2025-07-22.pdf).
- [CRA Standards Unlocked: Navigating Smartcards & Secure Elements](https://www.youtube.com/watch?v=zyVaaW0bNs4) (CEN-CLC JTC 13 WG 9, 25 Jul 2025) - How Annex IV critical products (smartcards, secure elements) achieve CRA compliance via EUCC. Slides: [`presentations/2025-07-25_webinar_cra-standards-unlocked-navigating-smartcards-secure-element-compliance-under-cra.pdf`](presentations/2025-07-25_webinar_cra-standards-unlocked-navigating-smartcards-secure-element-compliance-under-cra.pdf).
- [Unlocking CRA Security Controls — Preparation for Implementation](https://www.youtube.com/watch?v=br_iYoo9uak) (CEN TC 224 WG 17, 8 Sep 2025) - Practical steps manufacturers take to meet Annex I Part I (2) security controls. Slides: [`presentations/2025-09-08_webinar_unlocking_cra_security_controls_preparation_for_une_event.pdf`](presentations/2025-09-08_webinar_unlocking_cra_security_controls_preparation_for_une_event.pdf).
- [CRA Standards Unlocked: From IEC 62443 to CRA](https://www.youtube.com/watch?v=fClHoC_t44E) (CEN-CENELEC, 8 Sep 2025) - How an organisation already aligned with IEC 62443-4-1/4-2 can efficiently reach CRA compliance. Slides: [`presentations/2025-09-08_webinar_unlocking_cra_iec62443-series-for-cra.pdf`](presentations/2025-09-08_webinar_unlocking_cra_iec62443-series-for-cra.pdf).
- [CRA Standards Unlocked — Deep Dive (October 2025)](https://www.youtube.com/watch?v=_C9HGqBT6qw) (CEN-CENELEC, 13 Oct 2025) - Updated overview of CRA standards as essential-requirement drafts mature. Slides: [`presentations/2025-10-13_webinar_cra-standards-unlocked-navigating-smartcards-secure-element-compliance-under-cra.pdf`](presentations/2025-10-13_webinar_cra-standards-unlocked-navigating-smartcards-secure-element-compliance-under-cra.pdf).
- [CRA Standards Unlocked — Deep Dive (January 2026)](https://www.youtube.com/watch?v=mprdi2RSoww) (CEN-CENELEC, 22 Jan 2026) - Latest guidance as regulation approaches full application. Slides: [`presentations/2025-04-08_cyber-resilience-act-and-the-horizontal-standards-workshop.pdf`](presentations/2025-04-08_cyber-resilience-act-and-the-horizontal-standards-workshop.pdf).
- [Cybersecurity Requirements for Smart Meter Gateways](https://www.youtube.com/watch?v=z4aCSxbHdOU) (CEN-CENELEC, 23 Feb 2026) - Annex IV critical-product requirements for SMGW. Slides: [`presentations/2026-02-23_cra-standards-unlocked-cybersecurity-requirements-for-smgw_final.pdf`](presentations/2026-02-23_cra-standards-unlocked-cybersecurity-requirements-for-smgw_final.pdf).
- [Cybersecurity Requirements for Identity Management Systems](https://www.youtube.com/watch?v=mdldrP3Dq1M) (CEN-CENELEC, 25 Feb 2026) - Requirements for identity/privileged-access products (Annex III Class I). Slides: [`presentations/2026-02-25-webinar_cra-standards-unlocked-cybersecurity-requirements-for-identity-management-systems.pdf`](presentations/2026-02-25-webinar_cra-standards-unlocked-cybersecurity-requirements-for-identity-management-systems.pdf).
- [Deep Dive — Smart Meter Gateways (Part 1)](https://www.youtube.com/watch?v=oFdbyRgf7d4) (CEN-CENELEC, 2 Mar 2026) - Technical implementation for smart-meter gateways. Slides: [`presentations/2026-03-02_deepdive_part1-smartmeter-gateways.pdf`](presentations/2026-03-02_deepdive_part1-smartmeter-gateways.pdf).
- [Deep Dive — Generic Security Controls (prEN 40000-1-4)](https://www.youtube.com/watch?v=U0I4XVEje34) (CEN-CENELEC, 5 Mar 2026) - The horizontal security-controls standard applicable to every CRA product. Slides: [`presentations/2026-03-05_cra_unlocked_deepdive_securitycontrols_cen-clc-jtc-13-wg-9_pt2.pdf`](presentations/2026-03-05_cra_unlocked_deepdive_securitycontrols_cen-clc-jtc-13-wg-9_pt2.pdf).
- [Deep Dive — Identity Management Systems](https://www.youtube.com/watch?v=sPnvxDujEVg) (CEN-CLC JTC 13 WG 9, 18 Mar 2026) - Deeper technical analysis paired with the 25 Feb webinar. Slides: [`presentations/2026-03-18_cra_unlocked_cybersecurity_requirements_deep-dive_tc224wg17_cra.pdf`](presentations/2026-03-18_cra_unlocked_cybersecurity_requirements_deep-dive_tc224wg17_cra.pdf).

### ETSI Vertical-Standard Deep Dives (STAN4CRA)

Per-product-category deep dives produced by the STAN4CRA project for each ETSI EN 304-6xx draft.

- [Deep Dive — EN 304-617 Browsers](https://www.youtube.com/watch?v=RTYrnjoqzaw) (STAN4CRA / ETSI, 29 Jan 2026) - Standalone and embedded browsers. Slides: [`presentations/Browsers Deep Dive Session With Two Dans.pdf`](presentations/Browsers%20Deep%20Dive%20Session%20With%20Two%20Dans.pdf).
- [Deep Dive — EN 304-618 Password Managers](https://www.youtube.com/watch?v=IJC-70wlRHA) (STAN4CRA / ETSI, 19 Jan 2026) - Requirements for password manager products. Slides: [`presentations/Deep Dive Session on Password Managers.pdf`](presentations/Deep%20Dive%20Session%20on%20Password%20Managers.pdf).
- [Deep Dive — EN 304-619 Antivirus/Antimalware](https://www.youtube.com/watch?v=LEF9kcAkn5I) (STAN4CRA / ETSI, 29 Jan 2026) - Requirements for AV/anti-malware products. Slides: [`presentations/Cybersecurity requirements for software that searches for, removes, or quarantines malicious software. Deep Dive Session.pdf`](presentations/Cybersecurity%20requirements%20for%20software%20that%20searches%20for,%20removes,%20or%20quarantines%20malicious%20software.%20Deep%20Dive%20Session.pdf).
- [Deep Dive — EN 304-620 VPNs](https://www.youtube.com/watch?v=JXll0Qw0Yp4) (STAN4CRA / ETSI, 15 Jan 2026) - Virtual Private Network product requirements. Slides: [`presentations/Deep Dive Session on VPNs.pdf`](presentations/Deep%20Dive%20Session%20on%20VPNs.pdf).
- [Deep Dive — EN 304-622 SIEM](https://www.youtube.com/watch?v=3PKGpO0Fs-I) (STAN4CRA / ETSI, 26 Jan 2026) - Security Information and Event Management requirements. Slides: [`presentations/Cybersecurity requirements for security information and event management (SIEM) systems.pdf`](presentations/Cybersecurity%20requirements%20for%20security%20information%20and%20event%20management%20\(SIEM\)%20systems.pdf).
- [Deep Dive — EN 304-623 Boot Managers](https://www.youtube.com/watch?v=pVeg70coS5s) (STAN4CRA / ETSI, 19 Jan 2026) - Boot-manager requirements including UEFI. Slides: [`presentations/EN 304 623  Boot Managers Deep Dive Session.pdf`](presentations/EN%20304%20623%20%20Boot%20Managers%20Deep%20Dive%20Session.pdf).
- [Deep Dive — EN 304-624 PKI & Certificate Issuance](https://www.youtube.com/watch?v=Jq1D0VexKVc) (STAN4CRA / ETSI, 15 Jan 2026) - PKI and certificate-issuance software. Slides: [`presentations/Deep Dive Session on PKI and digital certificate issuance software.pdf`](presentations/Deep%20Dive%20Session%20on%20PKI%20and%20digital%20certificate%20issuance%20software.pdf).
- [Deep Dive — EN 304-624 Network Management Systems (NMS)](https://www.youtube.com/watch?v=Q8Pp3mk1Ne8) (STAN4CRA / ETSI, 29 Jan 2026) - Network-management product requirements. Slides: [`presentations/Deep Dive Session on Network Management Systems (NMS).pdf`](presentations/Deep%20Dive%20Session%20on%20Network%20Management%20Systems%20\(NMS\).pdf).
- [Deep Dive — EN 304-625 Physical/Virtual Network Interfaces](https://www.youtube.com/watch?v=SDeJE2Uf96k) (STAN4CRA / ETSI, 29 Jan 2026) - Network-interface product requirements. Slides: [`presentations/Deep Dive Session on Physical and Virtual Network Interfaces.pdf`](presentations/Deep%20Dive%20Session%20on%20Physical%20and%20Virtual%20Network%20Interfaces.pdf).
- [Deep Dive — EN 304-626 Operating Systems](https://www.youtube.com/watch?v=ByQSbsXCtdA) (STAN4CRA / ETSI, 26 Jan 2026) - CRA requirements for operating systems. Slides: [`presentations/Cybersecurity requirements for Operating Systems Deep Dive Session.pdf`](presentations/Cybersecurity%20requirements%20for%20Operating%20Systems%20Deep%20Dive%20Session.pdf).
- [Deep Dive — EN 304-627 Routers, Modems, Switches](https://www.youtube.com/watch?v=j5ND5vv8wZc) (STAN4CRA / ETSI, 17 Dec 2025) - Internet-facing routers, modems, switches. Slides: [`presentations/Cybersecurity requirements for routers, modems intended for the connection to the internet, and switches Deep Dive Session.pdf`](presentations/Cybersecurity%20requirements%20for%20routers,%20modems%20intended%20for%20the%20connection%20to%20the%20internet,%20and%20switches%20Deep%20Dive%20Session.pdf).
- [Deep Dive — EN 304-636 Firewalls, IDS/IPS](https://www.youtube.com/watch?v=XqSl61ud3PA) (STAN4CRA / ETSI, 22 Dec 2025) - Class II Important-product standard. Slides: [`presentations/Deep Dive Session on Firewalls.pdf`](presentations/Deep%20Dive%20Session%20on%20Firewalls.pdf).
- [Deep Dive — Consumer IoT Vertical Standards](https://www.youtube.com/watch?v=TyEIeUX2u-M) (STAN4CRA / ETSI, 9 Feb 2026) - Smart-home devices, connected toys, wearables. Slides: [`presentations/Deep dive session Consumer IoT Vertical Standards.pdf`](presentations/Deep%20dive%20session%20Consumer%20IoT%20Vertical%20Standards.pdf).
- **Deep Dive — Hardware Devices with Security Boxes** (STAN4CRA / ETSI) - HSM and dedicated-security-function products. *Recording URL not available;* slides: [`presentations/cra-standards-unlocked_deep-dive_cybersecurity-requirements-for-hardware-devices-with-security-boxes.pdf`](presentations/cra-standards-unlocked_deep-dive_cybersecurity-requirements-for-hardware-devices-with-security-boxes.pdf).
- **Deep Dive — Ivan TC224/WG17 CRA v4.1** (ETSI, 25 Jul 2025) - ETSI TC 224 WG 17 technical briefing. *Recording URL not available;* slides: [`presentations/2025-07-25_ivan_tc224wg17_cra_v41_webinar.pdf`](presentations/2025-07-25_ivan_tc224wg17_cra_v41_webinar.pdf).

### Q&A and Workshop Reports

- [CRA Unlocked Deep Dive — Q&A Report (13 Oct 2025)](presentations/q-a_report_webinar_cra_unlocked_deep_dive_2025-10-13.pdf) - Questions raised during the October 2025 deep-dive.
- [Smart Meter Gateways Webinar — Q&A Report (23 Feb 2026)](presentations/q-a_report_webinar_cra_unlocked_smart_meter_gateways_2026-02-23.pdf) - Questions from the SMGW webinar.
- [Q&A Report 01/08](presentations/qa-report-0108.pdf) - Additional aggregated Q&A.

---

## Relationship to Other EU Regulation

The CRA does not sit in isolation. These neighbouring regimes carve out, pre-empt, or overlap with CRA obligations.

- [NIS2 Directive (EU) 2022/2555](https://eur-lex.europa.eu/eli/dir/2022/2555/oj) - Covers essential and important *entities*. CRA covers *products*. Many manufacturers fall under both. NIS2 incident reporting (Art. 23) and CRA Art. 14 reporting run in parallel.
- [Radio Equipment Directive 2014/53/EU & Delegated Regulation (EU) 2022/30](https://ec.europa.eu/growth/sectors/electrical-engineering/red-directive_en) - RED cybersecurity requirements apply until 11 December 2027; then repealed in favour of the CRA. Local copy of the repeal act: [`docs/eu/red-delegated-act-repeal.pdf`](docs/eu/red-delegated-act-repeal.pdf).
- [Regulation (EU) 2024/1689 — AI Act](https://eur-lex.europa.eu/eli/reg/2024/1689/oj) - Art. 8 CRA coordinates with AI Act: products that are both high-risk AI systems and PDEs follow AI Act's conformity route, which CRA considers satisfied.
- [Regulation (EU) 2023/1230 — Machinery Regulation](https://eur-lex.europa.eu/eli/reg/2023/1230/oj) - Cybersecurity of safety-related machinery components. CRA generally excludes items covered by sector-specific cybersecurity rules (Art. 2(2)).
- [Regulation (EU) 2017/745 — Medical Devices (MDR)](https://eur-lex.europa.eu/eli/reg/2017/745/oj) - Excluded from CRA scope (Art. 2(2)(a)); MDR cybersecurity applies.
- [Regulation (EU) 2019/2144 — Vehicle General Safety](https://eur-lex.europa.eu/eli/reg/2019/2144/oj) and [UN R155](https://unece.org/transport/documents/2021/03/standards/un-regulation-no-155-cyber-security-and-cyber-security) - Vehicle cybersecurity is out of CRA scope; UN R155 + WP.29 apply instead.
- [Regulation (EU) 2016/679 — GDPR](https://eur-lex.europa.eu/eli/reg/2016/679/oj) - Data-protection complement. Security-of-processing (Art. 32 GDPR) and CRA essential requirements interact for any product processing personal data.
- [Cybersecurity Act (EU) 2019/881](https://eur-lex.europa.eu/eli/reg/2019/881/oj) - Framework under which the EUCC scheme is established; referenced by CRA Art. 8 and Art. 27(8)-(9).

---

## EU CRA Cluster Projects

Twelve EU-funded projects supporting CRA roll-out — from standards development to SME tooling. Managed via CYBERSTAND and SECURE initiatives.

- [CYBERSTAND](https://cyberstand.eu) - Cybersecurity Standardisation. Empowers European stakeholders to engage in CRA standards development. Selects 200+ experts with €1.5M funding for harmonised-standard working groups. Coordinates CEN/CENELEC/ETSI. *Primary gateway if you want to contribute to a standard.*
- [STAN4CRA](https://www.stan4cra.eu) - Standards for the Cyber Resilience Act. The ESO portal tracking all harmonised-standard development progress under M/606.
- [CRA-AI](https://cyberstand.eu/cra-cluster/cra-ai-cyber-resilience-act-and-artificial-intelligence) - AI-powered CRA compliance platform for product inventory, risk assessment, testing, documentation, vulnerability reporting. Focus on SME needs with training modules.
- [OSCRAT / OCCTET](https://occtet.eu) - Open-source CRA tooling: FOSS SBOM generation, vulnerability tracking, and automated compliance for open-source components in digital products.
- [CONFIRMATE](https://confirmate-project.eu) - Conformity assessment, metrics, compliance automation. Develops open-source tools on the Clouditor framework, penetration-testing methodology, multilingual training. Partners: Fraunhofer, CYEN, DNSC Romania.
- [CURIUM](https://curium-project.eu) - Cybersecurity resilience for IoT and microelectronics. Harmonised regulatory framework for ICT products under EUCSA and CRA; focus on certification of IoT and microelectronic components.
- [SECURE](https://www.secure4sme.eu) - €22M budget including €16M cascade funding for MSMEs. First open call January 2026 (€5M). Direct financial support, compliance tools, training for small businesses.
- [CRACoWi](https://www.cracowi.eu) - CRA Compliance Wizard. Step-by-step digital assistant guiding SMEs through secure design, lifecycle, and post-market compliance.
- [CYBERFORT](https://cyber-fort.eu) - Strengthening Cyber Defences of SMEs for CRA. Co-funded under Digital Europe Programme. Automated open-source compliance tools. Romania-Cyprus partnership coordinated by DNSC.
- [CRACY](https://cra-cy.eu) - CRA Made Easy. Consortium of 11 European cybersecurity technology providers. Belgium-Romania-Greece-Estonia partnership. Practical CRA tools for the supply chain.
- [TRUSTBOOST](https://www.trustboost.eu) - CyberBoost SaaS platform for real-time cybersecurity conformity and certification aligned with CRA, RED-DA, NIS2, CSA. Coordinated by NSAI (Ireland).

---

## Books & Long-Form References

These books are **copyrighted**. Links go to publishers or neutral reference pages; no content is hosted here.

- [Designing Secure Software: A Guide for Developers](https://nostarch.com/designing-secure-software) by Loren Kohnfelder — The engineering handbook behind CRA essential requirements. Part I covers the conceptual foundation (Trust, Authenticate/Authorize/Audit "Gold Standard", mitigation, design patterns, cryptography); Part II integrates security into design and the 6-step Security Design Review process that notified bodies will examine under Art. 32(2)(a); Part III drills into concrete practices — the GotoFail and Heartbleed case studies, untrusted-input handling, web security, security testing — that eliminate the vulnerability classes Annex I Part I (2)(a) targets. *Essential reading for engineers.* *(No Starch Press, 2021)*
- [Practical Vulnerability Management](https://nostarch.com/practical-vulnerability-management) by Andrew Magnusson — Operational handbook for running a vulnerability-management programme — exactly the day-to-day practice CRA Annex I Part II demands. Covers component and CVE data collection, Cull-Rank triage, the five response types (patch, mitigation, systemic, accept, defence-in-depth with validation), and PSIRT stakeholder management. Part II builds a working system with free tools (Nmap, OpenVAS, cve-search, Metasploit). *The operational playbook for Annex I Part II (1)-(8).* *(No Starch Press, 2020)*
- [Threat Modeling Best Practices](https://www.packtpub.com/en-ca/product/threat-modeling-best-practices-9781805129196) by Derek Fisher — 322-page engineering-facing threat-modelling handbook covering STRIDE, DREAD, ISO 27005, NIST SP 800-30, FAIR, OCTAVE, RMF; cloud/supply-chain/IoT/AI threat modelling with formal adversary models (Dolev-Yao, Byzantine, honest-but-curious); building a threat-modelling practice (SMART, maturity models, CoE/CoP). Maps directly onto CRA Art. 13(2) risk-assessment obligation. *(Packt Publishing, 2025)*
- [NIST SP 800-30 Rev. 1 — Guide for Conducting Risk Assessments](https://csrc.nist.gov/pubs/sp/800/30/r1/final) by NIST — The most widely-adopted risk-assessment methodology: threat identification, vulnerability analysis, likelihood, impact, risk determination. CRA Art. 13(2) requires a risk assessment, Art. 13(3) requires it documented and updated; NIST SP 800-30 provides a defensible structured approach. *Free PDF from NIST.* *(NIST, 2012)*
- [OWASP Developer Guide v4](https://devguide.owasp.org/) — Broad free developer guide covering secure-design principles, threat modelling, implementation, testing, operations. Useful complement to Kohnfelder. *Free; OWASP.*
- [OWASP CycloneDX — Authoritative Guide to SBOM](https://cyclonedx.org/guides/OWASP_CycloneDX-Authoritative-Guide-to-SBOM-en.pdf) — Free deep guide to SBOM production and consumption; directly relevant to Annex I Part II (1). *Free; OWASP.*

---

## Academic & Research

- [ENISA Threat Landscape (annual)](https://www.enisa.europa.eu/publications/enisa-threat-landscape-2024) - Annual assessment of the EU threat landscape; useful context for CRA risk assessments under Art. 13(2).
- [Joint Research Centre — CRA Publications](https://joint-research-centre.ec.europa.eu/) - JRC publishes technical analysis supporting Commission CRA policy.
- [SBOM research — Fraunhofer AISEC](https://www.aisec.fraunhofer.de/en/research.html) - Academic research on SBOM tooling and verification; frequently cited in ENISA SBOM study.
- [CVE / CWE / CAPEC (MITRE)](https://cve.mitre.org/) - The vulnerability-identifier ecosystem that every CRA PSIRT operates within.
- [FIRST CVSS v4.0](https://www.first.org/cvss/v4-0/) - The severity-scoring framework referenced throughout CRA vulnerability management.

---

## Community, Portals & Further Reading

- [European Commission — Cyber Resilience Act page](https://digital-strategy.ec.europa.eu/en/policies/cyber-resilience-act) - The official landing page. Bookmark.
- [DG CNECT](https://digital-strategy.ec.europa.eu/en) - Directorate-General for Communications Networks, Content and Technology — Commission team responsible for CRA.
- [ENISA CRA Hub](https://www.enisa.europa.eu/topics/cybersecurity-policy/cyber-resilience-act) - ENISA's CRA resource hub.
- [CCC — Consumer Choice Centre CRA analysis](https://consumerchoicecenter.org/) - Consumer-facing CRA commentary.
- [Eurosmart](https://www.eurosmart.com/) - Industry association for the digital security industry; publishes CRA conformity-assessment briefings.
- [DIGITALEUROPE](https://www.digitaleurope.org/) - Industry-side advocacy and CRA position papers.
- [BSA | The Software Alliance](https://www.bsa.org/) - Software-industry CRA analysis.
- [Open Source Initiative (OSI) — CRA pages](https://opensource.org/) - OSI commentary on Art. 2 (open-source scope) and Art. 24 (open-source stewards).
- [Eclipse Foundation CRA pages](https://cra.eclipse.org/) - Eclipse's CRA guidance for open-source communities.

---

## Contributing

Contributions are welcome. Please:

1. Read [CONTRIBUTING.md](CONTRIBUTING.md) first.
2. Only add **resources that are publicly available and relevant to the CRA** (regulation text, harmonised standards, official guidance, research, open-source tools, public webinars, books).
3. **Respect copyright:** link to the official catalogue page for paid standards and published books; do **not** submit PDF uploads of copyrighted material.
4. Follow the existing entry format: `- [Title](URL) - One or two factual sentences about the resource and its CRA relevance. *Paid/free/draft notes.*`
5. Keep descriptions factual, not promotional.
6. Open a pull request with a clear title (e.g., `add EN 304-624 deep-dive by STAN4CRA`).

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the maintainer has waived all copyright and related or neighbouring rights to this list. The curation and descriptions are released into the public domain via [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/).

The PDFs mirrored in `docs/eu/` and `presentations/` retain the rights of their original authors. EU publications are reused under [Commission Decision 2011/833/EU](https://eur-lex.europa.eu/eli/dec/2011/833/oj); presentation slides are mirrored as released by CEN, CENELEC, ETSI, ENISA, and the STAN4CRA/CYBERSTAND projects. If you are the rights-holder of any mirrored material and wish it removed, please open an issue.

---

## Maintainer

This list is curated and maintained by **Jeans Koo** at **The One Testing Technology Co., Ltd** — an ISO/IEC 17025 accredited testing laboratory supporting manufacturers through the EU Cyber Resilience Act lifecycle: scoping, risk assessment, security-by-design review, vulnerability management, and conformity assessment.

- 💼 [LinkedIn — Jeans Koo](https://www.linkedin.com/in/jeans-koo/)
- ✉️ [jeans.koo@theonelab.co](mailto:jeans.koo@theonelab.co)

*For questions, corrections, or to contribute a resource, open an issue or pull request — see [CONTRIBUTING.md](CONTRIBUTING.md).*

- [CausalLayer MCP](https://github.com/smq9sn5jck-coder/causallayer-mcp) - Deterministic liability attribution for AI systems, designed for EU regulatory compliance including AI Act and CRA overlap areas.
