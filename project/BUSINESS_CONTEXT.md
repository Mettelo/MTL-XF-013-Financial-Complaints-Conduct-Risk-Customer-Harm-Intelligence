# Business Context

## Business Problem

Conduct and complaints teams receive large volumes of complaint information, but headline complaint counts alone do not show whether customer outcomes are deteriorating. Large firms naturally generate more complaints, while smaller firms can have high complaint rates despite lower absolute volume. Upheld complaints, closure timeliness and product mix add further context, but these measures are often reviewed separately.

This creates a conduct-risk problem: leadership may overreact to high volume, miss smaller but persistent rate-based deterioration, or fail to identify products where several weak indicators are appearing at the same time.

The business problem is to create a governed complaints-intelligence view that separates scale from rate, combines multiple customer-outcome indicators and supports proportionate escalation decisions.

## Required Delivery Response

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

## How the Client Will Use the Output

The finished product should support a Conduct Risk Committee or complaints review. A senior manager should be able to ask: “Which product has both a high complaint rate and high upheld percentage?”, “Which firm has deteriorated for more than one reporting period?”, or “Where are slower closure times appearing alongside worsening complaint outcomes?”

The output should prioritise areas for investigation or monitoring. It must not describe an analytical flag as a regulatory breach, FCA finding or proven customer harm.

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
