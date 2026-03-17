# Hospitality Revenue Analytics – Power BI Dashboard

🌐 **Live Dashboard:**  
[View Dashboard](https://app.powerbi.com/view?r=eyJrIjoiMjhmYjg4N2YtYjVkYS00ZDVjLTlhN2QtOTY4MDk4ODU5OTZhIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

---

# Project Overview

This project presents an end-to-end **Revenue Analytics Dashboard** developed for **Evergreen Hospitality**, a multi-property hotel chain operating across India.

The objective was to analyze historical booking data and generate **actionable insights for the revenue management team** to improve:

- Occupancy
- Pricing strategy
- Revenue performance
- Customer experience

The solution enables stakeholders to identify performance gaps and implement **data-driven pricing and operational strategies**.

---

# Business Problem

Evergreen Hospitality has been experiencing:

- Declining **market share and revenue**
- Ineffective **pricing strategies**
- Lack of centralized analytics
- Poor visibility into:
  - Occupancy trends
  - Booking behavior
  - Platform performance
  - Customer satisfaction

The organization required a **data-driven solution** to optimize revenue management decisions.

---

# Solution

Developed a **Power BI dashboard** to:

- Track key hospitality KPIs
- Analyze booking and revenue trends
- Compare performance across properties, cities, and platforms
- Enable stakeholders to identify revenue leakage and optimization opportunities

---

# Dashboard Features

## Key KPIs

- Revenue
- RevPAR (Revenue per Available Room)
- ADR (Average Daily Rate)
- Occupancy %
- Realisation %
- Cancellation %
- DBRN (Daily Booked Room Nights)
- DSRN (Daily Sellable Room Nights)
- DURN (Daily Utilized Room Nights)

## Analytical Views

- **Trend Analysis**
  - Week-over-week performance of RevPAR, ADR, Occupancy %

- **Category Analysis**
  - Revenue split across Luxury vs Business hotels

- **Platform Analysis**
  - ADR and Realisation % across booking platforms

- **Property Performance**
  - Revenue, bookings, occupancy, ratings, cancellations

- **Day Type Analysis**
  - Weekday vs Weekend comparison

## Interactive Filters

- City
- Room Class
- Category
- Date (Weekly view)

---

# Data Model

The solution is built using a **Star Schema architecture**.

## Fact Tables

- fact_bookings  
- fact_aggregated_bookings  

## Dimension Tables

- dim_date  
- dim_hotels  
- dim_rooms  

This model enables efficient analysis across:

- Time
- Location
- Property
- Room category

---

# Data Transformation

Performed using **Power Query**:

- Data cleaning and standardization
- Handling missing values
- Data integration across multiple sources
- Relationship creation
- Column transformations

---

# Key Insights

## 1. Ineffective Pricing Strategy

- ADR remains relatively constant across weeks
- RevPAR fluctuates significantly

👉 Indicates a **static pricing strategy**

Since:

RevPAR = ADR × Occupancy

Fluctuation in RevPAR is driven by **occupancy changes**, not pricing.

### Recommendation:
- Implement **dynamic pricing strategies**
- Introduce **weekday vs weekend pricing**
- Adjust pricing based on demand trends

---

## 2. Low Occupancy Linked to Poor Ratings

- Low-performing properties show:
  - Low occupancy %
  - Low customer ratings
  - Higher cancellation %

👉 Strong correlation between **service quality and occupancy**

### Recommendation:
- Improve customer experience and service quality
- Focus on **low-performing properties (Pareto approach)**

---

## 3. Platform Pricing Inefficiencies

- ADR varies across platforms
- Realisation % remains similar

Observations:

- Highest ADR → Direct Offline
- Lowest ADR → Direct Online

👉 Direct channels are not fully optimized

### Recommendation:

Due to platform parity constraints:

- Use:
  - Coupons
  - Discounts
  - Loyalty offers
  - Bundled deals

👉 Increase occupancy via **indirect pricing strategies** to see a hike in revenue

---

## 4. Pricing vs Demand Relationship

- Inverse relationship observed between:
  - Pricing (ADR)
  - Occupancy

👉 Lower pricing can drive higher occupancy and overall revenue

### Recommendation:
- Apply **differential pricing strategies**
- Optimize based on demand elasticity

---

# Business Impact (Projected)

If implemented, the insights can lead to:

- Improved occupancy rates
- Better pricing optimization
- Increased revenue efficiency
- Reduced cancellations
- Enhanced customer satisfaction

---

# Tools & Technologies Used

- Power BI
- DAX
- Power Query
- Excel

---

# Screenshots

Dashboard screenshots are available in the `/screenshots` folder.

---

# Project Outcome

This project enables Evergreen Hospitality to transition from **static decision-making to data-driven revenue management**.

It provides a foundation for:

- Dynamic pricing strategies
- Operational improvements
- Strategic revenue growth

---

# Author

**Kamya Bhardwaj**
