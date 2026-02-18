# Data Cleaning & Preparation

All primary data cleaning and transformation procedures were executed in Google Sheets in accordance with capstone project requirements. The following structured data quality protocol was implemented prior to analytical modeling.

## Cleaning Steps Performed

All steps were executed with auditability and non-destructive operations where possible.

| Step | Issue Identified | Action Taken |
|:---|:---|:---|
| Duplicate Removal | Presence of duplicate transaction records | Identified and removed all duplicate rows using Google Sheets deduplication tools |
| Categorical Standardization | Inconsistent labels in `Item_Fat_Content` (e.g., 'LF', 'low fat', 'Low Fat') | Normalized all fat-content values to two standard labels: 'Low Fat' and 'Regular' |
| Whitespace Trimming | Extra leading/trailing spaces in categorical fields | Applied `TRIM()` across all text columns |
| Numeric Validation | Range validation conducted on `Item_Weight`, `Item_Visibility`, `Item_MRP`, `Item_Outlet_Sales` | Verified no negative or implausible values; flagged and reviewed outliers |
| Revenue Reconciliation | Validation of aggregated totals | Confirmed `SUM(Item_Outlet_Sales)` = ₹18,591,125.41 with zero unexplained variance |
| Structural Integrity | Orphaned or misclassified records | Cross-referenced all `Outlet_Identifier` values against outlet master table |

## Feature Engineering & Assumptions

- **Revenue Share %**: Derived by dividing category and format sales by total revenue; this KPI was not present in the raw dataset.
- **Average Sales per Item**: Computed as total format sales divided by item count to benchmark outlet efficiency.
- **Null handling (Item_Weight)**: Nulls in `Item_Weight` were treated as missing observations and excluded from weight-dependent analysis while retained for revenue calculations.

## Data Transformations

- Standardized categorical labels (e.g., `LF` → `Low Fat`)
- Trimmed whitespace inconsistencies using `TRIM()`
- Converted revenue fields to numeric aggregation format
- Derived percentage contribution metrics (category & outlet-format shares)

## Data Integrity Confirmation

Post-cleaning revenue totals remained unchanged at ₹18,591,125.41, confirming that all quality-control procedures were non-destructive. All findings in subsequent sections reflect actual transactional reality.

---

**Prepared in:** Google Sheets — Cleaning steps logged and exported to `Cleaned_Dataset_Folder/Retail Sales Analysis Clean Data.csv` for downstream analysis.

