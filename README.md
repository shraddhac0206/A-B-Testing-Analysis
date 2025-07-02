# A/B Testing Analysis: Landing Page Conversion Experiment

This project demonstrates the complete process of analyzing an A/B test to evaluate the effectiveness of a new landing page in improving user conversion rates. It uses real-world-style experimental data and applies data science techniques to clean, explore, test, and interpret the results. The analysis is performed using Python and well-known statistical libraries.

---

## Project Objective

The main goal of this A/B testing experiment is to determine whether the **new landing page design** results in a significantly higher conversion rate compared to the **old landing page**. A two-sample proportion Z-test is used to validate the statistical significance of any observed difference between the two groups.

---

## Dataset Overview

- `ab_data.csv`: Contains user-level data with columns such as `user_id`, `timestamp`, `group` (control/treatment), `landing_page`, and `converted` (1 = converted, 0 = not).
- Approximately 294,000 records representing a random split of users into control and treatment groups.

---

## Key Steps in the Notebook

1. **Data Cleaning**
   - Removed mismatched rows (e.g., control group with new page or vice versa).
   - Dropped duplicate user IDs to ensure experimental integrity.

2. **Exploratory Data Analysis (EDA)**
   - Assessed conversion rates by group and page type.
   - Explored user behavior trends over time using visualizations.
   - Conducted subgroup analyses (weekday vs. weekend, hourly patterns).

3. **Statistical Testing**
   - Performed a two-proportion Z-test to compare conversion rates.
   - Calculated p-value to determine statistical significance.
   - Conclusion drawn based on hypothesis testing.

4. **Insight Generation**
   - Identified subtle behavioral trends based on time and day.
   - Highlighted the importance of context (e.g., time of day) in A/B tests.

---

## Insights & Conclusion

Although the treatment group (new landing page) showed a slightly lower conversion rate than the control group, the difference was **not statistically significant**. Therefore, we cannot conclude that the new design improved conversions. However, the deeper time-based analysis revealed potential **opportunities for segmented testing** based on user activity patterns.

---

## Technologies Used

- **Python**: `pandas`, `numpy`, `matplotlib`, `seaborn`
- **Statistical Testing**: `scipy`, `statsmodels`
- **Jupyter Notebook**: Interactive, well-commented code execution

---

## How to Use This Project

1. Clone the repository:  
   `git clone https://github.com/shraddhac0206/ab-testing-landing-page.git`

2. Open the notebook file:  
   `ab_test_analysis_final.ipynb` in **Jupyter Notebook** or **Google Colab**

3. Run the notebook to reproduce the analysis, visualizations, and conclusions.

---

## Author & Contact

Created by **Shraddha Chauhan**  
If you have questions, suggestions, or want to collaborate, feel free to connect on [LinkedIn](https://www.linkedin.com) or email me at **shraddhachauhan261999@gmail.com**
