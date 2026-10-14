# 🎮 Xbox Ecosystem Strategy Analysis: Game Pass Ultimate & Hardware Economics (2020–2025)

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![DAX](https://img.shields.io/badge/DAX-00758F?style=for-the-badge&logo=microsoft&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

An end-to-end data analytics project evaluating the quantitative impact of major game releases (**Day One Game Pass** vs. **First-Party Non-Day One** vs. **Third-Party Control Group**) on Xbox Series X|S console hardware sales and **Xbox Game Pass Ultimate** subscriber adoption.

---

## 📌 Dashboard Preview
![Dashboard Preview](assets/dashboard_screenshot.png)

---

## 📖 Executive Summary & Context

Under Phil Spencer's leadership, Xbox shifted its growth paradigm from traditional hardware console sales to ecosystem expansion via **Xbox Game Pass Ultimate**. However, this strategy faces intense executive scrutiny: **Does Day One subscription access subsidize user acquisition at the expense of console hardware velocity and $70 full-price game sales?**

This analytical project explores 2020–2025 dataset trends to uncover the correlation between game release windows, hardware activation baselines, and long-term subscription compounding.

---

## 🎯 Key Analytical Findings

1. **Pre-Order Hardware Velocity Lift (+31.6%):**
   - Day One Game Pass releases drive an average of **4,449 console sales** in the pre-order-to-release window.
   - Compared to the non-Day One control baseline (**3,044.5 units** avg from 3,112 1st-Party + 2,977 3rd-Party), Day One releases yield a **+31.6% temporary lift** in console pre-orders.
2. **Hardware Baseline Ceiling (~1.5M Plateau):**
   - Despite high-profile 1st-party exclusives, long-term console hardware sales remain capped at a baseline plateau of **~1.5M cumulative lifetime units**, proving that exclusives shift purchase timing rather than expanding long-term total addressable hardware market (<5% overall baseline impact).
3. **Subscriber Compounding (35M Peak Base):**
   - Game Pass active subscriber base decoupled from flat hardware growth, scaling consistently to **35M active subscribers** with a **13M average steady baseline**.

---

## 💡 Strategic Recommendations & Roadmap

### 1. Singleplayer Day One Restructuring Options
To prevent subscription cannibalization on premium $200M+ AAA singleplayer titles:
* **Light Model:** Base launch version remains on Game Pass for 1 year, but excludes post-launch updates and DLCs (requires full purchase).
* **Mid Model (Recommended):** Time-banked campaign access based on average completion time (e.g., 8-hour access window for *Call of Duty*) or optional restriction on side-quests.
* **Aggressive Model (80% Progress Gate):** Story progress capped at 80% on Game Pass; final act/ending requires full title purchase.

### 2. Hardware & Multiplayer Pivots
* **Hardware Re-positioning:** Market Xbox console hardware as a budget PC workstation for emerging markets (supporting Full Keyboard/Mouse, office applications, and desktop UI mode).
* **Multiplayer Seasonal Access:** Game Pass Ultimate grants access **only to Season 1** of competitive multiplayer releases; ongoing participation requires title acquisition while driving Battle Pass & cosmetic upsells.

---

## 🛠 Tech Stack & Architecture

* **Data Generation & Processing:** Python (`pandas`, `numpy`)
* **Data Modeling:** Star Schema (Fact Tables: `fact_console_sales`, `fact_subscriptions`; Dimension Tables: `dim_games`, `dim_dates`)
* **Analytics & Visualization:** Power BI Desktop with custom DAX measures (`DIVIDE`, `CALCULATE`, `SAMEPERIODLASTYEAR`, `RANKX`).

---

## 📁 Repository Structure

```text
xbox-ecosystem-analytics/
├── assets/                  # Dashboard screenshots and slide previews
├── data/                    # Raw and processed datasets (CSV)
├── docs/                    # Full executive strategy presentation (PDF)
├── power_bi/                # Power BI (.pbix) report file and dax_measures.txt
├── scripts/                 # Python scripts for data ETL/generation
└── README.md                # Project documentation