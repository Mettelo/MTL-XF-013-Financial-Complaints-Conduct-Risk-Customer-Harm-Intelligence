# Project Brief

## 1. Business Problem

Conduct and complaints teams receive large volumes of complaint information, but headline complaint counts alone do not show whether customer outcomes are deteriorating. Large firms naturally generate more complaints, while smaller firms can have high complaint rates despite lower absolute volume. Upheld complaints, closure timeliness and product mix add further context, but these measures are often reviewed separately.

This creates a conduct-risk problem: leadership may overreact to high volume, miss smaller but persistent rate-based deterioration, or fail to identify products where several weak indicators are appearing at the same time.

The business problem is to create a governed complaints-intelligence view that separates scale from rate, combines multiple customer-outcome indicators and supports proportionate escalation decisions.

## What the Team Needs to Do

The team is expected to build a conduct and customer-harm intelligence solution using the FCA firm-level complaints data.

The work should include:
- defining the conduct-review and escalation questions;
- documenting firm, product, complaint and denominator/context fields;
- creating reproducible ingestion and standardisation from the FCA workbook;
- calculating complaint rates only where compatible denominators are available;
- analysing upheld percentage and closure performance alongside complaint volume;
- identifying persistent or material outliers;
- testing thresholds rather than choosing arbitrary cut-offs;
- creating a multi-indicator review framework;
- building BI that clearly separates volume, rate, upheld and closure measures;
- reconciling key figures back to the source;
- completing assurance, UAT and handover.

## Practical Use Case

The finished product should support a Conduct Risk Committee or complaints review. A senior manager should be able to ask: “Which product has both a high complaint rate and high upheld percentage?”, “Which firm has deteriorated for more than one reporting period?”, or “Where are slower closure times appearing alongside worsening complaint outcomes?”

The output should prioritise areas for investigation or monitoring. It must not describe an analytical flag as a regulatory breach, FCA finding or proven customer harm.

## 2. Business Decision
> **Which firms, products or complaint patterns should be escalated for conduct investigation, remediation review or enhanced monitoring, and what evidence is strong enough to justify that escalation?**

Charts without a defensible decision framework do not satisfy the commission.

## 3. Agreed Objectives
1. Create a governed firm/product complaints model from the FCA workbook.
2. Normalise volume measures using available contextual denominators so large firms are not automatically treated as worse performers.
3. Identify persistent or material combinations of high complaint rate, upheld rate and slow closure.
4. Create an interpretable conduct-review framework without presenting analytical flags as regulatory findings.
5. Provide a decision-support product for conduct, complaints and product-governance teams.

## 4. Key Business Questions
1. Which firms/products show unusually high complaint rates after accounting for available context?
2. Where are upheld percentages materially above peer or portfolio norms?
3. Which areas combine elevated complaints with slower closure performance?
4. Which outliers persist across product groupings or reporting periods available to the project?
5. Which data-quality or denominator limitations could materially change the interpretation?
6. What evidence should trigger investigation versus routine monitoring?

## 5. Cross-Functional Roles
| Role | Minimum expected output |
|---|---|
| Business Analyst | Define escalation use cases, stakeholder requirements, decision process and acceptance criteria. |
| Data Governance Analyst | Govern firm/product definitions, denominator rules, KPI ownership, lineage and DQ controls. |
| Data Engineer | Create reproducible workbook ingestion, standardisation and analytical tables. |
| Conduct/Data Analyst | Own complaint-rate, upheld, closure and outlier analysis. |
| BI Developer | Build conduct-monitoring dashboard with governed measures and drill-down. |
| Risk/Assurance Analyst | Own threshold challenge, reconciliation, UAT and interpretation controls. |

## 6. Minimum Delivery Standard
- traceable requirements and acceptance criteria;
- governed definitions, ownership, lineage and data-quality rules;
- preserved raw source and reproducible transformations;
- explicit reconciliation and exception handling;
- domain-specific analytical outputs;
- transparent prioritisation/intervention logic;
- governed stakeholder-facing BI;
- assurance/UAT evidence;
- reproducible handover and visible collaboration.

## 7. Constraints
- Complaint volume alone is not a conduct-risk measure because firm size and product exposure matter.
- An upheld complaint does not automatically prove systemic misconduct.
- FCA published data is aggregated and does not provide customer-level causal evidence.
- Comparisons must use compatible denominator/context fields and clearly state when these are unavailable.
- Analytical flags must not be described as FCA findings or enforcement conclusions.

## 8. Agreed Success Criteria
- Every rate metric documents its denominator; where a denominator is unavailable the metric is labelled as volume-only.
- At least five headline figures reconcile directly to the FCA source workbook for selected firms/products.
- No ranking uses raw complaint volume alone as a conduct-risk conclusion.
- Outlier thresholds are documented and sensitivity-tested.
- Firm/product identifiers and categories are standardised with an exception log.
- Dashboard users can distinguish volume, rate, upheld and closure measures without ambiguous labels.

## 9. Out of Scope
Core delivery does not require confidential customer-level data, paid production infrastructure, automated operational decisions or unsupported causal inference.

## 10. Reproducibility Definition
A reviewer should be able to clone the team repository, obtain the documented approved source data, run the workflow and reproduce the curated analytical outputs and validation evidence without undocumented manual changes.
