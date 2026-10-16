# Project Brief

## Engagement Details

| Field | Detail |
|---|---|
| Project ID | MTL-XF-013 |
| Project Title | Financial Complaints, Conduct Risk & Customer Harm Intelligence |
| Client | Confidential Regulated Financial Services Group |
| Sector | Financial Services / Conduct / Customer Outcomes |
| Duration | 8 weeks |
| Recommended Team Size | 6–8 |
| Primary Sponsor | Director of Conduct Risk |
| Senior Stakeholders | Head of Complaints, Consumer Duty Lead, Product Governance Lead, Operational Risk Lead, Compliance Monitoring Lead, Data Governance Lead, BI & Analytics Lead |
| Primary Dataset | FCA Firm-Specific Complaints Data — 2025 H2 |

## 1. Client Situation
Senior management receives complaint totals, but volume, upheld rate, closure timeliness and contextual denominators are reviewed separately. This makes it difficult to distinguish scale effects from genuine deterioration in customer outcomes or conduct risk.

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
