# Data Guidance

## Approved Core Dataset

Use the FCA **Firm-Specific Complaints Data — 2025 H2** workbook.

Official source:
https://www.fca.org.uk/data/complaints-data/firm-level

The workbook contains the firm-level tables used for:
- complaints opened;
- complaints closed;
- closure timing;
- upheld percentage;
- context measures;
- product groups;
- joint-reporting information.

## Raw File

Store the original downloaded workbook unchanged:

```text
data/raw/
└── fca-firm-level-complaints-2025-h2.xlsx
```

Do not export and overwrite the source workbook as your only raw copy.

## Core Reporting Period

Use **2025 H2: 1 July to 31 December 2025** as the mandatory frozen cohort.

This is sufficient for the core cross-sectional conduct-risk exercise.

## Recommended Historical Extension

For persistence/trend analysis, add prior half-year files from the FCA archive:
- 2025 H1;
- 2024 H2;
- optionally 2024 H1.

Official historical page:
https://www.fca.org.uk/data/complaints-data/previous-complaints-data

Recommended trend scope: **at least 4 half-year periods** if the team is making claims about persistence.

Do not describe a one-period outlier as a persistent issue.

## Important Workbook Handling

The workbook may contain:
- multiple product-group tabs;
- context fields with different meanings;
- joint reporters;
- notes/definitions.

Teams must:
1. identify the correct sheet(s);
2. preserve firm identifiers/names;
3. document product-group mapping;
4. document which context denominator is used for each complaint-rate metric;
5. retain notes about joint reporters.

## Small vs Larger Working Data

The raw XLSX is manageable enough to keep directly in GitHub.

Processed analytical CSV/Parquet outputs should go in `data/processed/`, not replace the source workbook.

## Optional Aggregate Data

The FCA also publishes aggregate complaint tables. These may be used for validation or context but should not replace the firm-level workbook for this project.
