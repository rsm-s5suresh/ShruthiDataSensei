Objective:
This project focuses on implementing uplift modeling to enhance the effectiveness of targeted marketing campaigns. Unlike traditional propensity-to-buy models, which predict the likelihood of a customer 
making a purchase, uplift modeling estimates the incremental impact of an advertisement by identifying customers who are more likely to convert because of the ad rather than independent of it.The goal is to 
leverage machine learning techniques to maximize incremental revenue by selecting the most responsive customers for the Zalon campaign, thereby optimizing marketing spend and improving ROI.

Approach:
Data Preparation:

1. Two customer groups were used:
   Control Group (cg_organic_control) – 30,000 customers who did not receive an ad.
   Treatment Group (cg_ad_random) – 30,000 randomly selected customers who received an ad.
   A combined dataset was created with an indicator variable (ad = 1 for treated, ad = 0 for control).
   Data was split into training (70%) and test (30%) sets while maintaining balanced distributions.

2. Modeling & Evaluation:

   Uplift Model Implementation:
   Logistic Regression was trained to predict responses separately for the treatment and control groups.
   Uplift scores were computed as the difference between treatment and control predictions.
   Model performance was assessed using uplift tables and incremental uplift plots.

3. Comparison with Propensity Models:
   A traditional propensity-to-buy model was developed for benchmarking. The incremental revenue of targeting the top 30,000 customers using each model was compared.

4. Advanced Machine Learning Models:
   Neural Network, Random Forest, and XGBoost models were trained and tuned to improve uplift predictions.

5. Optimizing Customer Targeting Strategy:
   Instead of targeting a fixed 25% of customers, an optimal percentage was determined using uplift-driven decision-making.The best-performing model was used to maximize expected profit from customer selection.
