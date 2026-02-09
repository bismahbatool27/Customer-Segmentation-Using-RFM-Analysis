# 📊 Customer-Segmentation-Using-RFM-Analysis

## Project Overview
This project performs **RFM (Recency, Frequency, Monetary) analysis** on an online retail dataset to understand customer purchasing behavior.  
The goal is to segment customers into meaningful groups (Platinum, Loyal, Potential, At Risk, Lost) and suggest marketing strategies for each group.

---

## Dataset
- Columns used: 
  - CustomerID
  - InvoiceDate
  - Quantity
  - UnitPrice

---

## Approach

1. **Data Cleaning**
   - Removed rows with missing CustomerID
   - Removed negative quantities (returns)
   - Created a Monetory column (Quantity × UnitPrice)

2. **RFM Calculation**
   - **Recency:** Days since last purchase
   - **Frequency:** Number of invoices per customer
   - **Monetory:** Total money spent

3. 🎯 **RFM Scoring**
   - Scores (1–5) assigned based on quantiles
   - Recency is reversed (recent buyers score higher)
   - Frequency & Monetory: higher is better

4. **Customer Segmentation**
   - Applied rules to classify customers:
     - Champions, Loyal, Potential, At Risk, Lost

5. **Analysis & Visualization**
   - Segment distribution
   - Segment summary (average R, F, M + customer count)

---

## Results

- Number of customers in each segment:

| Segment           | Customer Count |
|------------------|----------------|
| Champions         | X              |
| Loyal Customers   | X              |
| Potential         | X              |
| At Risk           | X              |
| Lost Customers    | X              |

---

## Marketing Recommendations

| Segment           | Strategy |
|------------------|----------|
| Platinum          | Exclusive offers, early access, loyalty rewards |
| Loyal Customers   | Discount bundles, personalized recommendations |
| Potential         | First-time buyer discounts, onboarding emails |
| At Risk           | Win-back campaigns, limited-time discounts |
| Lost Customers    | Re-engagement emails, surveys |

## 📈 Visualizations

### 🔹 Customer Segment Distribution
Horizontal bar chart showing the number of customers in each segment.

---

### 🔹 RFM Metrics with Customer Counts
- Bar chart: Average of **Recency, Frequency, Monetary**
- Line plot: **Customer count**
