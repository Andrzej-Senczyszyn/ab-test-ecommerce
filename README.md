# E-commerce A/B Test (Portfolio Project)

This project analyzes an A/B test of an e-commerce landing page (`old_page` vs `new_page`).

---

## Project Steps
1. **Load & preview raw data** (`ab_data.csv`).
2. **Data cleaning:**
   - Removed mismatched rows (e.g., control → new_page, treatment → old_page).
   - Dropped duplicate users by `user_id` (kept the first occurrence).
3. **Group balance check** (~50/50 expected).
4. **Conversion rate (CR)** calculation for each group.
5. **Two-proportion Z-test** with 95% confidence interval.
6. **Visualization:** CR by group.
7. **(Bonus)** Daily CR trend analysis.
8. **Summary & business conclusion.**

---

## Key Results (from this dataset)
- CR (control): **12.04%**  
- CR (treatment): **11.88%**  
- Relative uplift: **−1.31%**  
- p-value: **0.1899**  
- 95% CI (treatment − control): **[−0.39%, +0.08%]**

---

## Conclusion
The treatment group shows a slightly lower conversion rate than the control group.  
The difference is **not statistically significant** (p ≥ 0.05).  
👉 We do **not have enough evidence** to say that the new landing page performs better than the old one.

---

## How to Run
1. Clone this repository.  
2. Open the notebook: `notebook/ecommerce_ab_test_EN_READY.ipynb`.  
3. Run cells to reproduce the analysis.  
  

---

## Tools & Libraries
- Python  
- pandas  
- matplotlib  
- statsmodels  

---

