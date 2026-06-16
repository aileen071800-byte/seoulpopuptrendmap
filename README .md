# Seoul Pop-up Store Trend Map — Dataset

**Research by Jooeun Lim · SKKU Department of Dance · 2024–2026**

This repository contains the structured datasets powering the *Seoul Pop-up Trend Map 2024–2026* Streamlit dashboard.

---

## ⚠️ Data Verification Notice

| Year | Status |
|------|--------|
| 2024 | ✅ **Actual** — based on Popga 2024 full dataset (1,431 entries) |
| 2025 | ⚠️ **Estimated** — based on 2024 trend trajectory + ~22% YoY growth (Popga, DealSeoul) |
| 2026 | ⚠️ **Estimated** — extrapolated from 2025 observed trends (IP surge, beauty expansion) |

Individual pop-up entries for 2025–2026 are drawn from **verified brand announcements and field research** by Jooeun Lim.
National share percentages for 2025–2026 are **estimates, not official statistics**.

---

## Files

### 1. `seoul_popups_main.csv` — 78 entries
The core dataset. Each row is one pop-up store researched and documented by Jooeun Lim.

| Column | Description |
|---|---|
| `district_no` | District number (01–05) |
| `district` | Full district name |
| `district_key` | Key: seongsu / hannam / hongdae / gangnam / others |
| `year` | Year: 2024, 2025, or 2026 |
| `category` | IP · Character / Fashion / Beauty / F&B / Art · Exhibition / Lifestyle |
| `popup_name` | Name of the pop-up |
| `brand` | Brand or organiser |
| `description` | What the pop-up offered |
| `location` | Specific address or area |
| `date` | Date or period of operation |
| `admission` | Free / Paid admission |
| `goods` | Goods or services available |
| `tags` | Keywords separated by ` \| ` |
| `highlight` | HOT / Notable / Major / Standard etc. |
| `research_insight` | Strategic analysis note by Jooeun Lim |

---

### 2. `national_category_share_2024_2026.csv` — 21 rows
Category share % of the total national pop-up market.

| Column | Description |
|---|---|
| `year` | 2024 / 2025 / 2026 |
| `data_type` | `Actual` or `Estimated` |
| `is_verified` | `YES` (actual) or `NO — ESTIMATED` |
| `category` | Category name |
| `share_pct` | Percentage share of all national pop-ups |
| `count_approx` | Approximate count = total × share% |
| `total_nationwide` | Total pop-up count nationwide |
| `estimation_method` | How the value was derived |
| `source` | Data source |

> ⚠️ Only 2024 values are verified. 2025 and 2026 are estimates.

---

### 3. `district_summary.csv` — 14 rows
Pop-up counts per district per year (based on this dataset).

| Column | Description |
|---|---|
| `district_no` | Sort key (01–05) |
| `district` | District full name |
| `district_subtitle` | Korean subtitle |
| `district_key` | Short key |
| `year` | Year |
| `popup_count_in_dataset` | Count of pop-ups in this dataset |
| `color_hex` | Brand color used in dashboard |

---

### 4. `key_trends_2024_2026.csv` — 6 rows
Six headline trend observations distilled from the research.

| Column | Description |
|---|---|
| `stat` | Headline statistic (e.g. "21%", "52%", "NEW") |
| `title` | Trend name |
| `description` | Full trend description |
| `source` | Data source |

---

## Data Sources

- **Popga (팝가)** — Korea's largest pop-up tracking platform (1,431 entries, 2024 full year) ✅ Verified
- **Seongsu Gorilla** — Seongsu district specialist tracker ✅ Verified
- **Inside Seoul** — Seoul pop-up news and analysis ✅ Verified
- **DealSeoul** — Community analytics and trend data ✅ Verified
- **Field Research** — Personal visits to Seongsu-dong and Hannam-dong by Jooeun Lim ✅ Verified
- **2025–2026 national figures** — Trend-based estimates ⚠️ Not officially verified

---

## License

For academic and educational use. Please credit:
> *Jooeun Lim, SKKU Department of Dance, Seoul Pop-up Trend Map 2024–2026*
