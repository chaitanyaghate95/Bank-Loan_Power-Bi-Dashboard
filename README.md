# 🏦 Bank Loan Analytics Dashboard — Power BI

> An advanced, multi-dashboard Power BI solution for comprehensive bank loan data analysis, enabling data-driven decision-making across lending operations.

---

## 📌 Project Overview

Traditional loan reporting methods often fail to provide interactive, real-time insights into lending operations. This project addresses that gap by building a **suite of interconnected Power BI dashboards** that deliver dynamic and comprehensive insights into loan data — empowering stakeholders with actionable intelligence derived from robust data analysis.

---

## 🎯 Objective

To craft a set of interconnected dashboards offering a **holistic perspective** on:

- Lending operations performance
- Borrower demographics and behavior
- Loan performance and risk classification
- Financial health metrics (interest rates, DTI, funded amounts)

---

## 📊 Dashboards

### 1. 📋 Executive Summary
High-level KPI overview for evaluating the overall efficiency and performance of lending operations.

| KPI | Total | MTD | MoM Change |
|-----|-------|-----|------------|
| Total Loan Applications | 38.6K | 4.3K | +6.9% |
| Total Funded Amount | $435.8M | $54.0M | +13.0% |
| Total Amount Received | $473.1M | $58.1M | +15.8% |
| Average Interest Rate | 12.0% | 12.4% | +3.5% |
| Average DTI | 13.3% | 13.7% | +2.7% |

**Key Features:**
- Month-to-Date (MTD) and Month-over-Month (MoM) tracking for all major KPIs
- Good Loan vs Bad Loan classification with funded and received amount breakdowns
- Loan status table: Fully Paid, Charged Off, and Current

---

### 2. 🗺️ Overview
Trend and distribution analysis across multiple dimensions.

**Visualizations include:**
- **Monthly Trend** — Total loan applications by month (Jan–Dec)
- **Geographic Distribution** — Applications by U.S. state
- **Loan Term Split** — 36-month (73.2%) vs 60-month (26.8%) distribution
- **Employment Length** — Breakdown from `< 1 year` to `10+ years`
- **Loan Purpose** — Debt consolidation, credit card, home improvement, etc.
- **Home Ownership** — RENT (18K), MORTGAGE (17K), and other categories

---

### 3. 🔍 Details
Granular record-level view with full loan metadata.

| Field | Description |
|-------|-------------|
| Loan ID | Unique loan identifier |
| Purpose | Reason for loan (e.g., debt consolidation, credit card) |
| Home Ownership | Rent / Mortgage / Own |
| Grade & Sub-Grade | Risk classification (A–G) |
| Issue Date | Loan origination date |
| Funded Amount | Total disbursed amount |
| Interest Rate | Applied interest rate |
| Installment | Monthly repayment amount |
| Amount Received | Total repayment collected |

---

## 🟢 Good Loan vs 🔴 Bad Loan Classification

| Category | Metric |
|----------|--------|
| Good Loans | 86.2% of total funded and received amount |
| Bad Loans (Charged Off) | 13.8% of total funded and received amount |
| Fully Paid | 32,145 applications — $351.4M funded |
| Charged Off | 5,333 applications — $65.5M funded |
| Current | 1,098 applications — $18.9M funded |

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Power BI Desktop** | Dashboard development and data visualization |
| **DAX** | KPI calculations, MTD/MoM measures |
| **Power Query (M)** | Data transformation and cleaning |
| **Excel / CSV** | Source data format |

---

## 📁 Project Structure

```
bank-loan-analytics/
│
├── 📂 data/
│   └── bank_loan_data.csv          # Raw loan dataset
│
├── 📂 reports/
│   └── Bank_Loan_Analytics.pbix    # Main Power BI report file
│
├── 📂 documentation/
│   └── Bank_Loan_Analytics_Report.docx  # Project report and KPI definitions
│
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites
- [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (latest version recommended)

### Steps to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/bank-loan-analytics.git
   cd bank-loan-analytics
   ```

2. **Open the report**
   - Launch Power BI Desktop
   - Open `reports/Bank_Loan_Analytics.pbix`

3. **Connect your data** *(if using your own dataset)*
   - Go to **Home → Transform Data**
   - Update the data source path to point to your local CSV file

4. **Refresh & Explore**
   - Click **Refresh** to load the latest data
   - Navigate across the **Summary**, **Overview**, and **Details** tabs

---

## 📈 Key Insights

- Loan applications show a **consistent upward trend** from January through December
- **Debt consolidation** is the most common loan purpose (~18K applications)
- Borrowers with **10+ years of employment** represent the largest applicant segment (8.9K)
- The majority of borrowers are **renters or mortgage holders**
- **86.2% of loans** are classified as "Good Loans" (Fully Paid or Current)

---

## 💼 Use Cases

- **Bank Management** — Monitor overall lending performance and portfolio health
- **Risk Analysts** — Track bad loan rates and charged-off amounts
- **Loan Officers** — Understand borrower demographics and loan purpose trends
- **Finance Teams** — Assess cash inflows and funded amount patterns

---

## 🤝 Contributing

Contributions are welcome! If you'd like to improve the dashboards or add new features:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-dashboard`)
3. Commit your changes (`git commit -m 'Add new dashboard'`)
4. Push to the branch (`git push origin feature/new-dashboard`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 📬 Contact

For questions or collaboration, feel free to reach out via [GitHub Issues](https://github.com/your-username/bank-loan-analytics/issues).

---

> ⭐ If you found this project helpful, please consider giving it a star!
