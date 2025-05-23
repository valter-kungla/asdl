# Autonomous Software Development Levels (ASDL)

> *A technology‑neutral standard for describing the maturity of autonomy in the
> software‑engineering lifecycle – inspired by the SAE J3016 self‑driving‑car
> levels.*

**Version 1.0 – 23 May 2025**  
**Authors**  • ChatGPT (OpenAI o3) — original specification • Valter Kungla

---

## Purpose

ASDL offers a concise vocabulary (L0 → L5) for teams, vendors, researchers and
regulators to communicate **how much of the software‑development process is
handled autonomously by AI agents versus humans.**  The intent is to:

* set clear expectations for risk & governance,
* enable benchmarking of tooling, and
* provide a road‑map for incremental adoption of autonomous capabilities.

---

## Quick Reference Table

| Level | Tag line                           | Human role                              | Primary AI capabilities                          |
|------:|------------------------------------|-----------------------------------------|--------------------------------------------------|
| **L0** | *Manual*                           | Writes **all** code, tests, infra, docs | none (editor/Lint only)                          |
| **L1** | *Assisted*                         | Accepts/rejects micro‑suggestions       | context autocompletion, style lint, simple unit‑test stubs |
| **L2** | *Partial*                          | Reviews & integrates AI output          | whole‑function generation, refactors, unit‑/integration‑test generation, CI/CD hooks |
| **L3** | *Conditional*                      | Sets goals, approves PRs, intervenes    | multi‑step planning, feature branches, self‑test loop, auto‑PRs, infra templating |
| **L4** | *High*                             | Monitors dashboards, handles edge cases | end‑to‑end feature delivery, architectural choices, canary+auto‑rollback deploys, self‑healing infra |
| **L5** | *Full*                             | Strategic governance only               | self‑directed road‑mapping, continuous self‑improvement, multi‑agent verification, dynamic infra evolution |

---

## Detailed Level Definitions

### **L0 – No Automation**
* **Coding**  Human writes 100 % of source.
* **Testing**  Manual or scripted by human.
* **Architecture & Design**  Fully human.
* **Deployment/Ops**  Triggered and monitored by humans.
* **Oversight**  Intrinsic – human is the actor.

### **L1 – Assisted Development**
* **Coding**  AI suggests tokens/lines; developer confirms.
* **Testing**  Tools scaffold basic unit‑test templates.
* **Code Review**  Linters/static‑analysis bots comment on style & obvious defects.
* **Ops**  Rule‑based CI/CD; AI not trusted to merge or deploy.

### **L2 – Partial Automation**
* **Coding**  AI generates complete functions/modules on request.
* **Testing**  AI proposes unit & happy‑path integration tests; dev curates.
* **Architecture**  AI recommends patterns; human chooses.
* **Deployment**  Pipeline can auto‑deploy to staging; prod gated by human.
* **Oversight**  Human reviews every PR; AI cannot merge.

### **L3 – Conditional Automation**
* **Scope**  AI agents execute multi‑step feature tasks (“add profile API”).
* **Quality Loop**  Agents write code ➜ generate tests ➜ run ➜ fix until green.
* **Code Review**  AI summarises changes; human approves/high‑level review.
* **Deployment**  To prod with human sign‑off or policy‑based auto‑merge.
* **Infra**  Agents provision resources via IaC within budget/policy.
* **Fallback**  Human can halt/override at any step.

### **L4 – High Automation**
* **End‑to‑End Delivery**  Given a requirement, agents design, code, test,
  document, and deploy.
* **Release Engineering**  AI selects rollout strategy, monitors SLOs, auto‑
  rolls back on anomalies.
* **Self‑Healing**  Detects & patches most runtime issues without waiting for
  humans.
* **Architecture**  Makes bounded architectural changes (e.g., splits
  microservice) respecting org constraints.
* **Human Duty**  Define objectives, constraints & handle rare edge cases.

### **L5 – Full Autonomy**
* **AGI‑level Capability**  AI originates product ideas, performs research,
  architects novel systems, writes and maintains code indefinitely.
* **Continuous Optimization**  Live‑experiments, auto‑tuning of cost vs.
  latency, dynamic infra migration.
* **Governance**  Human provides only strategic/ethical guard‑rails; routine
  development & ops are self‑governed.
* **Accountability Mechanisms**  AI logs rationale, proofs, and audit trails for
  regulatory or ethical scrutiny.

---

## Conformance Checklist

To **claim** a given level you must satisfy **all** lower‑level criteria plus the
additional capabilities listed for that level.  Organizations can publish a
self‑assessment table like:

| Capability                            | L0 | L1 | L2 | L3 | L4 | L5 |
|---------------------------------------|:--:|:--:|:--:|:--:|:--:|:--:|
| AI generates entire functions         |    | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ |
| Agent opens autonomous PRs            |    |    |    | ✔️ | ✔️ | ✔️ |
| **Human‑free production deploy**      |    |    |    |    | ✔️ | ✔️ |
| AI sets its **own** development goals |    |    |    |    |    | ✔️ |

> *Tip – include proof links (demo videos, audit logs) for each ✔️ in real
> assessments.*

---

## Road‑map Guidance

1. **Inventory today’s tooling** – map each to ASDL levels.
2. **Define risk appetite** – higher autonomy ⇒ stronger safety nets
   (formal verification, RLAIF, guard‑rails).
3. **Increment progressively** – pilot L2 in low‑risk repos before aiming for
   L3+, etc.
4. **Track metrics** – time‑to‑merge, defect rate, MTTR; expect step‑changes at
   each level.

---

## Relationship to Other Standards
* ASDL is intended to complement, not replace, existing software development methodologies, quality standards (e.g., ISO/IEC 25010 for software product quality), or process models (e.g., CMMI).
* Its specific focus is on classifying the degree of autonomy in the software engineering lifecycle, providing a common language for this particular dimension.
* Users are encouraged to integrate ASDL concepts within their broader quality assurance and development frameworks.

---

## Versioning and Evolution
* This ASDL specification follows semantic versioning (e.g., v1.0, v1.1, v2.0).
* Major versions (e.g., v1.x to v2.x) introduce significant changes or conceptual shifts that may not be backward compatible.
* Minor versions (e.g., v1.0 to v1.1) introduce backward-compatible clarifications, additions, or refinements.
* Proposals for changes, new levels, or clarifications can be submitted via GitHub Issues for discussion. Significant changes will be incorporated into new minor or major versions after community review and consensus.
* The version of the standard is indicated at the top of this document.

---

## License (MIT)

---

## How to Contribute

1. Fork ➜ create feature branch ➜ submit a PR.
2. Fill the **conformance checklist** for any new capability.
3. Sign your commits & ensure CI passes.
4. By contributing you agree that your code/content is licensed MIT.

We look forward to your contributions.
