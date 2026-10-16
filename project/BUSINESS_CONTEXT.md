# Business Context

## Simulated Client
**Confidential Regulated Financial Services Group**

## Current Problem
Senior management receives complaint totals, but volume, upheld rate, closure timeliness and contextual denominators are reviewed separately. This makes it difficult to distinguish scale effects from genuine deterioration in customer outcomes or conduct risk.

## Decision Owner
**Director of Conduct Risk**

## Senior Stakeholders
Head of Complaints, Consumer Duty Lead, Product Governance Lead, Operational Risk Lead, Compliance Monitoring Lead, Data Governance Lead, BI & Analytics Lead

## Decision
**Which firms, products or complaint patterns should be escalated for conduct investigation, remediation review or enhanced monitoring, and what evidence is strong enough to justify that escalation?**

## Role Responsibilities
| Role | Required contribution |
|---|---|
| Business Analyst | Define escalation use cases, stakeholder requirements, decision process and acceptance criteria. |
| Data Governance Analyst | Govern firm/product definitions, denominator rules, KPI ownership, lineage and DQ controls. |
| Data Engineer | Create reproducible workbook ingestion, standardisation and analytical tables. |
| Conduct/Data Analyst | Own complaint-rate, upheld, closure and outlier analysis. |
| BI Developer | Build conduct-monitoring dashboard with governed measures and drill-down. |
| Risk/Assurance Analyst | Own threshold challenge, reconciliation, UAT and interpretation controls. |

## Evidence Chain
**Requirement → governed definition → transformation → quality control → metric/analysis → decision insight → recommendation → UAT**

Major recommendations must be traceable through this chain.
