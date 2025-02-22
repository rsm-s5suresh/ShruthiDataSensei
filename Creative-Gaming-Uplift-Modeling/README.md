# Creative Gaming Uplift Modeling

## 📌 Objective
This project focuses on implementing **uplift modeling** to enhance the effectiveness of targeted marketing campaigns. Unlike traditional **propensity-to-buy models**, which predict the likelihood of a customer making a purchase, **uplift modeling** estimates the **incremental impact** of an advertisement by identifying customers who are more likely to convert **because of the ad**, rather than independently.

The goal is to leverage **machine learning techniques** to **maximize incremental revenue** by selecting the most responsive customers for the **Zalon campaign**, thereby optimizing **marketing spend** and improving **ROI**.

---

## 🛠 Approach

### **📂 Data Preparation**
1. **Two customer groups were used:**
   - **Control Group (`cg_organic_control`)** – 30,000 customers who **did not receive an ad**.
   - **Treatment Group (`cg_ad_random`)** – 30,000 randomly selected customers who **received an ad**.
2. A combined dataset was created with an **indicator variable** (`ad = 1` for treated, `ad = 0` for control).
3. The dataset was split into **training (70%) and test (30%) sets**, ensuring balanced distributions.

---

### **📊 Modeling & Evaluation**
#### ✅ **Uplift Model Implementation**
- **Logistic Regression** was trained to predict responses separately for the **treatment** and **control** groups.
- **Uplift scores** were computed as the difference between treatment and control predictions.
- Model performance was assessed using **uplift tables** and **incremental uplift plots**.

#### 🔄 **Comparison with Propensity Models**
- A traditional **propensity-to-buy model** was developed for benchmarking.
- The **incremental revenue** of targeting the **top 30,000 customers** using each model was compared.

#### 🚀 **Advanced Machine Learning Models**
To improve uplift predictions, the following models were trained and optimized:
- **Neural Network**
- **Random Forest**
- **XGBoost**

---

### **🎯 Optimizing Customer Targeting Strategy**
- Instead of targeting a **fixed 25%** of customers, an **optimal percentage** was determined using **uplift-driven decision-making**.
- The **best-performing model** was selected to **maximize expected profit** from customer selection.

---

## 📌 **Key Takeaways**
✅ Uplift modeling helps optimize **ad targeting** by identifying **causal** impact.  
✅ Machine learning models like **XGBoost** and **Neural Networks** improve uplift prediction accuracy.  
✅ **Incremental revenue analysis** ensures marketing spend is directed towards **high-value customers**.  

---

## 🛠 **Technologies & Tools Used**
- **Python, SQL**
- **scikit-learn, XGBoost**
- **pandas, NumPy, matplotlib, seaborn**
- **A/B Testing, Causal Inference, Uplift Modeling**


