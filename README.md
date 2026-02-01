# Tuneworks-EDA-SQL
# TuneWorks-Operations-Customer-Insights

This project analyzes the operational performance, customer behavior, and revenue drivers of an entertainment booking agency (TuneWorks) using advanced SQL techniques applied to transactional business data.

---

## 1. Research Objective

The primary objective of this project is to evaluate TuneWorks’ operational efficiency, customer loyalty, and revenue concentration, and to identify strategic opportunities for improving profitability and scalability.

Specifically, we aim to answer the following questions:

- How efficiently are agents and entertainers utilized over time?
- Which customers and cities contribute the most to revenue and long-term value?
- Are customer entertainment preferences aligned with current entertainer offerings?
- Where do operational risks (e.g., scheduling conflicts, workload imbalance) arise?

---

## 2. Methodology

### Data & Setup
- **Dataset:** TuneWorks Entertainment Booking Database  
- **Timeframe:** September 2017 – March 2018  
- **Core Tables:** Agents, Customers, Entertainers, Engagements  
- **Supporting Tables:** Musical styles, customer preferences, calendar reference tables  

### Key Analytical Techniques
- Multi-table joins across transactional and reference data
- Aggregation and segmentation using `GROUP BY` and `HAVING`
- Window functions (`LAG`, `RANK`, `ROW_NUMBER`) for temporal and workload analysis
- Time-based analysis using `DATE_TRUNC`, quarterly indexing, and gap calculations
- Outlier detection using the Interquartile Range (IQR) method
- Customer growth analysis using Compound Quarterly Growth Rate (CQGR)

### Data Quality Handling
- Identification of missing engagement records and incomplete entertainer profiles
- Median imputation for extreme salary and commission outliers
- Documentation of ambiguous fields requiring client clarification

---

## 3. Key Findings

### Customer & Revenue Insights
- 100% of customers are repeat clients, indicating exceptionally strong customer loyalty
- A small subset of customers accounts for a disproportionate share of total revenue
- High-value cities (e.g., Bellevue, Auburn) generate strong revenue even with fewer bookings

### Content & Customer Fit
- Several high-spending customers prefer musical styles not currently represented by the entertainer pool
- Certain styles (e.g., Country, 60’s Music) are both high-demand and high-margin
- Other styles show high frequency but low average contract value, indicating limited pricing power

### Operational Efficiency
- Significant agent workload imbalance, with some agents overbooked and others underutilized
- One critical entertainer scheduling overlap identified, posing reputational risk
- Extremely short turnaround times between engagements suggest operational strain

### Customer Growth & Lifetime Value
- Rapid spending growth observed among a small number of customers (CQGR > 2.0)
- Top customers exhibit distinct style and entertainer preferences
- These customers represent strong candidates for loyalty and premium service programs

---

## 4. Conclusion

The analysis reveals that TuneWorks benefits from a highly loyal and profitable customer base, but faces structural limitations due to geographic concentration, flat incentive structures, and operational inefficiencies.

Key strategic takeaways include:
- The need to rebalance agent workloads and modernize compensation structures
- Opportunities to increase margins by focusing on high-value customers and cities
- Clear evidence that aligning entertainer supply with customer preferences could unlock additional revenue

---

## Repository Contents


---

## Notes

This project was completed as part of **DSO 555: Advanced SQL for Business Analysts**  
at the **University of Southern California**.
