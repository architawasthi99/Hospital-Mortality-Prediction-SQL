# Hospital Mortality Dashboard — Power BI Build Specification

## Source
Use `Hospital_Mortality_PowerBI_Source.xlsx` and import all sheets.

## Page title
HOSPITAL MORTALITY DASHBOARD

## Recommended visuals
1. Patient Count by Age Group — horizontal bar chart — Age Group[Age Interval] + Patient Count.
2. Deaths & Survivals in Each ICU Admit Source — clustered column chart — ICU Admit Source + Deaths + Survivals.
3. Patient Count for Each BMI Category — horizontal bar chart — BMI Category + Patient Count.
4. Average L.O.S in Each ICU Type — clustered column chart — ICU Type + LOS (Death) + LOS (Survived).
5. Rate of Death From Each Comorbidity (out of 100) — donut chart — Comorbidity + Death Rate / 100.
6. Death Rate For Each Ethnicity (out of 100) — donut chart — Ethnicity + Death Rate / 100.
7. Death Percentage by Age Group — table/matrix — Age Group + Death Percentage.
8. Amount of Deaths & Average Age From Each ICU Type — table — ICU Type + Amount That Died + Avg Age.
9. Hospital Death Statistics — cards/table — Mortality Rate % and Total Hospital Deaths.

## KPI values visible in screenshot
Mortality Rate: 6.34%
Total Hospital Deaths: 634

## Styling
- Canvas: 16:9
- Background: near-black (#050505)
- Accent: orange (#F28E2B)
- Secondary series: muted blue (#5B8DB8)
- Titles: orange, bold
- Data labels: white/light gray
- Use the supplied JSON theme for a close visual match.

## Important limitation
This is a reconstruction from the screenshot. It does not contain the original patient-level rows, so Power BI cannot reproduce arbitrary slicers or recompute every metric from the underlying patients. For a fully interactive dashboard based on your SQL queries, the original `ps_data` CSV/Excel/database table is required.
