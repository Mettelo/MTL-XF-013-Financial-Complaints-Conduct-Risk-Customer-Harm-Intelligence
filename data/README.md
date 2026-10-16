# Data Guidance

## Approved Core Dataset

Use the FCA **Firm-Specific Complaints Data — 2025 H2** workbook.

Official source:
https://www.fca.org.uk/data/complaints-data/firm-level

The workbook includes firm-level complaint information for:
- complaints opened;
- complaints closed;
- closure timing;
- upheld percentage;
- context measures;
- product groups;
- joint-reporting information.

## Raw File

Store the original workbook unchanged:

```text
data/raw/
└── fca-firm-level-complaints-2025-h2.xlsx
```

Do not overwrite the source workbook with a cleaned version.

## Core Reporting Period

Mandatory frozen cohort:
**2025 H2 — 1 July to 31 December 2025**

This is sufficient for the core cross-sectional conduct-risk work.

## Recommended Historical Extension

For persistence/trend analysis, add prior half-year files from:
https://www.fca.org.uk/data/complaints-data/previous-complaints-data

Recommended:
- 2025 H1;
- 2024 H2;
- optionally 2024 H1.

Use at least **4 half-year periods** before describing an issue as persistent.

## Workbook Handling

Before analysis:
1. identify the required sheet(s);
2. preserve firm names/identifiers;
3. document product-group mapping;
4. document the denominator/context field used for each rate;
5. retain joint-reporter notes.

## Recommended Grain

Use a clearly documented firm × product-group × reporting-period grain.

Do not combine incompatible context measures.

## Processed Data

Derived CSV/Parquet outputs belong in `data/processed/`.

Keep the original XLSX as the frozen raw source.

## Optional Aggregate Data

FCA aggregate complaints tables may be used for validation/context, but they should not replace the firm-level source.
