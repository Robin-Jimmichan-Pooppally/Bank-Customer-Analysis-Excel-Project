# 🏦 Bank Customer Segmentation Analysis Dashboard – Demographics & Subscription Insights

[![Excel](https://img.shields.io/badge/Excel-Dashboard-green?logo=microsoft-excel)](https://www.microsoft.com/excel)
[![Customer Analytics](https://img.shields.io/badge/Type-Segmentation_Analysis-blue)](https://github.com)
[![Subscription Trends](https://img.shields.io/badge/Analysis-Customer_Behavior-orange)](https://github.com)

A comprehensive Excel solution built to analyze bank customers by demographics and account balance to understand subscription behavior. It transforms customer-level data into actionable insights — enabling teams to identify subscription patterns across age groups, job categories, marital status, and balance ranges, with multilevel segmentation providing granular insights for targeted marketing and customer strategies.

---

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Project Objective](#project-objective)
- [Dataset Description](#dataset-description)
- [Tools & Techniques Used](#tools--techniques-used)
- [Pivot Tables & Visuals](#pivot-tables--visuals)
- [Installation & Prerequisites](#installation--prerequisites)
- [How to Use](#how-to-use)
- [Key Findings](#key-findings)
- [Tech Stack](#tech-stack)
- [Skills Demonstrated](#skills-demonstrated)

---

## 📊 Project Overview

This Excel project provides an **interactive analysis of customer segmentation and subscription behavior** using pivot tables, pivot charts, and conditional formatting. It enables monitoring of:

- 📈 **Overall subscription distribution** (Subscribed vs Not Subscribed)
- 👥 **Subscription rate by age group** (Campaign conversion across age demographics)
- 💼 **Subscription rate by job category** (Conversion by job function)
- 💍 **Subscription trends by marital status** (Subscription patterns by relationship status)
- 💰 **Balance range distribution** (Customer portfolio by account balance)
- 🎯 **Multilevel segmentation** (Job → Marital → Age_Group with subscription intensity)

---

## 🎯 Project Objective

To analyze bank customers by demographics and account balance to understand subscription behavior:

✅ **Identify subscription patterns** across customer demographics  
✅ **Segment customers** by age, job, marital status, and balance range  
✅ **Calculate subscription rates** by customer segment  
✅ **Highlight high-subscription segments** for targeted marketing  
✅ **Provide granular customer insights** for strategic planning  
✅ **Support data-driven targeting** for campaign optimization  

---

## ⚙️ Tools & Techniques Used

| Tool | Purpose |
|------|---------|
| **Microsoft Excel** | Data organization, pivot tables, dashboard creation |
| **PivotTables** | Customer segmentation and subscription aggregation |
| **PivotCharts** | Visual subscription trends (Donut, Stacked Bar, Pie charts) |
| **Calculated Fields** | Percentage-of-total and subscription rate calculations |
| **Conditional Formatting** | Color-coded intensity mapping (5-color legend) |
| **Slicers** | Dynamic filtering capability across dimensions |

---

## 📁 Dataset Description

### Dataset Overview

Customer-level records aggregated into pivot tables with counts and percentage-of-total values for subscription analysis.

### Columns Used

| Column | Description |
|--------|-------------|
| **CustomerID** | Unique customer identifier |
| **Age_Group** | Age category (18–25, 26–35, 36–45, 46–55, 56+) |
| **Job** | Job category (Admin, Blue-collar, Management, Retired, Self-employed, Services, Technician) |
| **Marital** | Marital status (Single, Married, Divorced) |
| **Balance_Range** | Account balance category (Low, Medium, High) |
| **Status of Subscription** | Subscription status (Subscribed, Not Subscribed) |

---

## 📈 Pivot Tables & Visuals

### 1️⃣ Overall Customer Subscription Distribution

**Chart Type:** Donut Chart

**Pivot Configuration:**
- **Rows:** Status of Subscription
- **Values:** Count of CustomerID (shown as percentage of total)

**Exact Distribution:**

| Status | Percentage |
|--------|-----------|
| **Not Subscribed** | 76.04% |
| **Subscribed** | 23.96% |

**Insight:** Approximately 24% of customers are subscribed; 76% are not subscribed.

---

### 2️⃣ Age-wise Campaign Conversion

**Chart Type:** Stacked Horizontal Bar

**Pivot Configuration:**
- **Rows:** Age_Group
- **Columns:** Status of Subscription
- **Values:** Count of CustomerID shown as % of Row Total

**Exact Percentages by Age Group:**

| Age Group | Not Subscribed | Subscribed |
|-----------|----------------|-----------|
| **18–25** | 76.40% | 23.60% |
| **26–35** | 74.78% | 25.22% |
| **36–45** | 77.80% | 22.20% |
| **46–55** | 76.68% | 23.32% |
| **56+** | 74.38% | 25.62% |

**Insight:** 26–35 and 56+ age groups show the highest subscription rates (~25.2% and 25.6% respectively). 36–45 group shows the lowest subscription rate (~22.20%).

---

### 3️⃣ Campaign Conversion by Job Category

**Chart Type:** Stacked Horizontal Bar

**Pivot Configuration:**
- **Rows:** Job
- **Columns:** Status of Subscription
- **Values:** Count of CustomerID shown as % of Row Total

**Exact Percentages by Job:**

| Job Category | Not Subscribed | Subscribed |
|--------------|----------------|-----------|
| **Admin** | 75.46% | 24.54% |
| **Blue-collar** | 75.37% | 24.63% |
| **Management** | 78.43% | 21.57% |
| **Retired** | 74.83% | 25.17% |
| **Self-employed** | 75.43% | 24.57% |
| **Services** | 76.93% | 23.07% |
| **Technician** | 75.88% | 24.12% |

**Insight:** Most job groups cluster in the mid-20% subscription range. Management shows the lowest subscription share (~21.57%). Retired and Self-employed show relatively higher subscription shares (~25%).

---

### 4️⃣ Subscription Trends by Marital Status

**Chart Type:** Stacked Horizontal Bar

**Pivot Configuration:**
- **Rows:** Marital
- **Columns:** Status of Subscription
- **Values:** Count of CustomerID shown as % of Row Total

**Exact Percentages by Marital Status:**

| Marital Status | Not Subscribed | Subscribed |
|----------------|----------------|-----------|
| **Divorced** | 77.23% | 22.77% |
| **Married** | 75.85% | 24.15% |
| **Single** | 75.04% | 24.96% |

**Insight:** Differences are small across marital groups. Divorced shows lower subscription (22.77%) vs Single (~24.96%) and Married (~24.15%).

---

### 5️⃣ Balance_Range Distribution

**Chart Type:** Pie Chart

**Pivot Configuration:**
- **Rows:** Balance_Range
- **Values:** Count of CustomerID shown as percentage of total customers

**Exact Distribution:**

| Balance Range | Percentage of Customers |
|--------------|------------------------|
| **Medium** | 49.30% |
| **High** | 25.74% |
| **Low** | 24.96% |

**Insight:** Medium balance customers are the largest group (nearly half the sample). High and Low balance groups are roughly equal (~25.7% and ~24.96%).

---

### 6️⃣ Multilevel Pivot (Job → Marital → Age_Group) with Subscription % + Colour Coding

**Pivot Configuration (Structure):**
- **Rows (Hierarchy):** Job → Marital → Age_Group
- **Columns:** Balance_Range (High / Low / Medium)
- **Values:** Count of CustomerID per balance range + Subscription Rate (%)

**Formatting & Color Legend:**

The final percentage column is color-coded with a 5-color legend:

| Color | Label |
|-------|-------|
| **Red** | Very Low |
| **Orange** | Low |
| **Yellow** | Medium |
| **Light Green** | High |
| **Dark Green** | Very High |

**Sample Data Rows (Job · Marital · Age_Group → High Count · Low Count · Medium Count → Subscription Rate):**

- Admin · Divorced · 18–25 → 6 · 6 · 17 → 0.42%
- Admin · Divorced · 26–35 → 14 · 16 · 15 → 0.30%
- Admin · Divorced · 36–45 → 18 · 4 · 26 → 0.52%
- Blue-collar · Single · 26–35 → 11 · 15 · 33 → 0.66%
- Management · Single · 26–35 → 20 · 16 · 30 → 0.60%
- Self-employed · Married · 26–35 → 15 · 10 · 42 → 0.84%
- Technician · Married · 26–35 → 15 · 9 · 22 → 0.44%

**Insight:** The detailed multilevel pivot presents subscription intensity per Job–Marital–Age_Group cell. Color-coding highlights segments with higher subscription rates. Examples: Self-employed / Married / 26–35 shows a higher rate (~0.84%); many other cells show lower percentages.

---

## ⚙️ Installation & Prerequisites

### System Requirements

- **Microsoft Excel** (2016 or later recommended)
- **Windows 10** or later / **macOS** with Excel installed
- **2GB RAM** minimum (4GB+ recommended)
- **100MB** free disk space

### Installation Steps

```
1. Download the Excel File
   → Bank-Customer-Segmentation-Dashboard-[Excel].xlsx

2. Open Microsoft Excel

3. File → Open → Select Bank-Customer-Segmentation-Dashboard-[Excel].xlsx

4. Wait for file to load completely

5. Navigate to Dashboard sheet to view visuals
```

---

## 📊 How to Use

### Accessing the Dashboard

**Step 1: Open the File**
```
Microsoft Excel → File → Open → Bank-Customer-Segmentation-Dashboard-[Excel].xlsx
```

**Step 2: Navigate to Dashboard Sheet**
- Select the Dashboard tab/sheet from the sheet tabs at the bottom
- All visualizations and metrics are displayed on this sheet

**Step 3: Use Interactive Elements**

| Feature | Action |
|---------|--------|
| **Overall Subscription Donut** | View overall subscription distribution at a glance |
| **Age-wise Stacked Bar** | Analyze subscription conversion by age group |
| **Job Category Stacked Bar** | Compare subscription rates across job functions |
| **Marital Status Stacked Bar** | Review subscription patterns by marital status |
| **Balance Range Pie Chart** | Understand customer portfolio distribution |
| **Multilevel Pivot** | Explore granular Job–Marital–Age segments with color-coded subscription intensity |
| **Color Legend** | Reference 5-color mapping (Very Low to Very High) for subscription intensity |

### Interpreting the Data

- **Overall Donut Chart** → High-level subscription penetration overview
- **Age-wise Stacked Bar** → Which age groups have higher subscription rates
- **Job Category Stacked Bar** → Job function subscription performance
- **Marital Status Stacked Bar** → Marital segment subscription trends
- **Balance Range Pie** → Distribution of customers across balance categories
- **Multilevel Pivot Table** → Granular cell-level subscription intensity for targeted actions
- **Color Coding** → Quick visual identification of high-subscription segments

---

## 💡 Key Findings

### Overall Subscription

✅ **Overall subscription rate: ~23.96%** subscribed; 76.04% not subscribed

✅ **Low penetration** indicates opportunity for targeted subscription campaigns

### Age Group Insights

✅ **26–35 and 56+ age groups** show the highest subscription rates (~25.2% and 25.6% respectively)

✅ **36–45 age group** shows the lowest subscription rate (~22.20%)

✅ **Age variation modest** — all groups cluster within 3-4% range

### Job Category Insights

✅ **Management shows lowest** subscription share (~21.57%) among listed jobs

✅ **Retired and Self-employed** show relatively higher subscription shares (~25%)

✅ **Most job groups cluster** in mid-20% subscription range

### Marital Status Insights

✅ **Single customers** show highest subscription (~24.96%)

✅ **Divorced customers** show lower subscription (~22.77%)

✅ **Marital differences are small** — only 2% spread across groups

### Balance Range Insights

✅ **Medium balance customers** are the largest group (49.30% of portfolio)

✅ **High and Low balance groups** are roughly equal (~25.7% and ~24.96%)

✅ **Nearly half the sample** in Medium balance category

### Multilevel Segmentation Insights

✅ **Granular segments** identified through Job–Marital–Age_Group breakdown

✅ **Higher subscription cells** highlighted in green (Light Green / Dark Green colors)

✅ **Color-coded intensity** enables visual identification of high-potential segments

---

## 🧰 Tech Stack

| Component | Technology |
|-----------|------------|
| **Platform** | Microsoft Excel |
| **Analysis Tool** | PivotTables & PivotCharts |
| **Data Visualization** | Excel Charts (Donut, Stacked Bar, Pie) |
| **Calculation** | Percentage-of-total and subscription rate formulas |
| **Formatting** | Conditional Formatting (5-color legend) |
| **Data Source** | Customer-level bank data |

---

## 📁 Project Files

**File:** `Bank-Customer-Segmentation-Dashboard-[Excel].xlsx`
- Excel workbook with customer data and interactive dashboard
- Contains pivot tables, pivot charts, conditional formatting, and segmentation analysis
- Ready for immediate use and customer targeting strategy

---

## 💼 Skills Demonstrated

✅ **PivotTable Creation** for multi-dimensional customer analysis  
✅ **PivotChart Design** for subscription trend visualization  
✅ **Calculated Fields** for percentage and subscription metrics  
✅ **Conditional Formatting** for color-coded intensity mapping  
✅ **Data Aggregation** by multiple dimensions (Job, Marital, Age)  
✅ **Customer Segmentation** analysis and insights  
✅ **Dashboard Design** with coordinated visuals  
✅ **Subscription Behavior** analysis and interpretation  
✅ **Data Visualization** for customer insights  
✅ **Targeted Marketing** support through segmentation  

---

## 📝 Notes

- Dataset contains customer-level records aggregated into pivot tables
- All pivot tables use Count of CustomerID as primary aggregation metric
- Subscription percentages displayed are derived from customer counts
- Conditional formatting uses 5-color legend mapping for visual intensity
- Multilevel pivot shows raw counts by Balance_Range with computed subscription rates
- Color mapping enables quick identification of high-subscription customer segments
- Analysis supports targeted marketing campaigns and customer strategy development
- All pivot configurations reproducible through standard Excel PivotTable functionality

---

*This Excel-based Bank Customer Segmentation Analysis Dashboard demonstrates practical customer analytics expertise, combining customer-level data aggregation through pivot tables, multi-dimensional segmentation analysis, and conditional formatting visualization to enable data-driven decision-making through comprehensive monitoring of subscription behavior patterns, demographic insights, balance distribution, and granular Job–Marital–Age segment identification for targeted marketing optimization.*
