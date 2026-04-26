# Real Estate Sales Performance & Customer Insights Dashboard

## 1. Background & Overview
### Context
In the real estate market, fragmented sales data often prevents businesses from accurately tracking occupancy rates and identifying target customer segments. This project standardizes transaction data across multiple buildings to provide a comprehensive view of business performance.

### Objectives
* **Trend Analysis:** Monitor revenue and sales volume trends over time (Year/Month).
* **Product Efficiency:** Analyze performance differences between Apartments and Offices.
* **Customer Profiling:** Map demographics (Age, Purpose, Source) to optimize marketing campaigns.

### Business Questions
| Dimension | Question |
| :--- | :--- |
| **WHEN** | What is the revenue trend by year? Which months are peak-selling season? |
| **WHAT** | Which building has the highest occupancy? What is the unsold inventory profile? |
| **WHO** | Which age group drives the most revenue? Do they buy to live or invest? |
| **HOW** | Which marketing channel brings the most units and highest satisfaction? |

---

## 2. Data Structure & Processing
**Data Source:**
* Practice dataset from **365 Data Science**.
* The dataset includes information on apartment code, building, selling price, area, customer information (Age, Country), and source.

**Data Cleaning**
| Issue Found | Action Taken |
| :--- | :--- |
| 72 blank Status rows (unsold inventory) | Filled → "Available" |
| Customers purchase information (M, D) for Firms are blank | Filled → "N/A" |
| Variables in wrong data types (Year, Month, D/M/Y) | Converted to correct data types (Number/Date) |

---

## 3. Dashboard Preview
![Real Estate Sales Dashboard](Real%20estate%20sales_Dashboard.png)

---

## 4. Insight Deep Dive
* **Sales Seasonality:** Revenue consistently peaks at the end of the year (**November peak**). This indicates a strong trend of home-buying or investment sentiment before the transition to the new year.
* **Customer Persona:** * The **36 - 45 age group** is the primary revenue driver, showing a significantly higher inclination toward **Investment** compared to younger segments.
    * Interestingly, the **18-25 age group**, despite having the lowest sales volume (5 units), boasts the **highest average price per unit**. This suggests that young buyers are specifically targeting premium properties or high-end segments.
* **Product Efficiency:** Although **Offices** occupy a larger average area, their contribution to total revenue is substantially lower than **Apartments**. This provides a solid basis for the business to reconsider floor space allocation in future projects.
* **Source Effectiveness:** **Website** and **Agency** are the two highest-quality channels, accounting for the vast majority of successful transactions.
