# Bitcoin Market Sentiment Analysis 📊

---

## **Overview**
This project explores how **market sentiment**, **trade-level metadata**, and **temporal behavior** influence Bitcoin trading outcomes. 
Instead of relying on predefined patterns or rigid assumptions, the analysis is entirely data-driven, allowing insights to emerge organically from raw trading data.

---

## **Key Objectives**
*   **Predict trade direction** using sentiment and trade metadata.
*   **Estimate Expected Profit & Loss (PnL)**.
*   **Identify key drivers of profitability** using explainable AI.
*   **Segment traders** into behavioral personas.
*   **Detect latent market regimes** using deep learning.

---

## **Dataset Description**
The dataset consists of merged trading and sentiment data, including:
*   **Fear–Greed Index values**
*   **Trade execution details**
*   **Fees, position size, and realized PnL**
*   **Timestamped market activity**

---

## **Project Workflow**

### **1. Data Preprocessing**
*   **Temporal Features:** Timestamp parsing into hour, weekday, and month.
*   **Data Cleaning:** Handling missing values using statistical imputers.
*   **Encoding:** Categorical features handled with One-Hot Encoding.
*   **Scaling:** Feature scaling for clustering and deep learning.

---

### **2. Trade Direction Prediction**
*   **Model:** Random Forest Classifier
*   **Inputs:** Market sentiment, Trade size & execution details, Temporal features.
*   **Outcome:** Demonstrates a strong relationship between sentiment and trade direction.

---

### **3. Expected PnL Modeling**

#### **Formula-Based Expected PnL**
A deterministic Expected PnL function was designed to act as a ground-truth baseline:

$$ Expected\_PnL = \frac{(Closed\_PnL - Fee)}{Start\_Position} \times Sentiment\_Value $$

#### **Model-Based Expected PnL**
*   **Model:** Random Forest Regressor
*   **Goal:** Comparing ML predictions against the logic-based formula to evaluate volatility and noise.

---

### **4. Explainability with SHAP**
*   Applied **SHAP values** to identify what drives profit.
*   **Key Drivers:** Trade timing and execution features ranked higher than pure sentiment.

---

### **5. Trader Behavior Clustering**
*   **Model:** KMeans
*   **Identified Personas:** 
    *   *Efficient Traders* (High profit, low fee)
    *   *Fearful Traders* (Low sentiment impact)
    *   *Aggressive Traders* (High volume)

---

### **6. Market Regime Detection (Deep Learning)**
*   **Model:** LSTM Autoencoder
*   **Insight:** Reveals hidden market transitions not visible in raw price data.

---

## **Visual Outputs**
*   📈 **Expected PnL vs Market Sentiment**
*   📅 **Seasonal profitability trends**
*   🧬 **SHAP feature importance summaries**
*   👥 **Trader behavior clusters**

---

## **Tech Stack**
*   **Python** (Pandas, Scikit-Learn, TensorFlow/Keras)
*   **Explainable AI**: SHAP
*   **Visualization**: Seaborn & Matplotlib

---

## **Author**
### **Kavya Bhardwaj**
**AI / ML | Data Science | Market Analytics**

🔗 **GitHub Project Link:** https://github.com/kavyabhardwaj2004/ds_Kavya_Bhardwaj
