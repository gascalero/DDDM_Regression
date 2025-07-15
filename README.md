This project developed a **data-driven model to accurately estimate house prices** for Cuckoo Cribs, moving away from guesswork. Built using **Knime Analytics Platform**, the model aims to help real estate agents make faster, more informed decisions and identify good deals.

**Key Aspects of the Model:**
*   **Data & Features:** The model uses real historical housing data. **Important numerical variables (like OverallQual, GrLivArea, GarageCars) were selected based on their high correlation with 'SalePrice'**, while irrelevant categorical variables were removed.
*   **Model Choice:** An **advanced Gradient Boosted Trees model** was chosen for its **high accuracy** by combining many small models, its proven industry use, and its clear, reviewable results.
*   **Performance:** The model shows **strong results**.
    *   **R² of 0.91**: It explains 91% of house price changes.
    *   **Mean Absolute Error (MAE): $14,584**: On average, predictions are within $14,584 of the real price.
    *   **Mean Absolute Percentage Error (MAPE): 8.5%**: The average error is a low 8.5% of the real price.

**Business Impact & Value:**
*   **Increased Accuracy & Confidence**: Cuckoo Cribs can price properties more accurately, leading to higher revenue and reduced business risk.
*   **Reduced Pricing Mistakes**: Helps avoid overpricing or underpricing, improving profits.
*   **Tangible Savings**: Can prevent losses from undervalued sales (e.g., $200,000 for 10 homes), reduce market time and holding costs (saving $1,000-$2,000 per property), and help identify undervalued properties for investments.

**Deployment & Maintenance:**
*   **User Interface**: Recommended to be integrated into a **simple, user-friendly interface** (web dashboard or mobile app) for agents.
*   **Agent Use**: Agents can use it for instant price estimates, client consultations, lead prioritization, and training.
*   **Monitoring & Retraining**: Continuous monitoring of performance (using RMSE, MAE, MAPE) and data drift is crucial. **Scheduled retraining every 3 to 6 months** with updated data, or condition-based retraining if performance drops (e.g., MAPE exceeds 10%), is enabled by a **KNIME workflow for minimal manual intervention**.

**Future Improvements**: Exploring other models (like XGBoost), integrating explainability tools (SHAP/LIME), and implementing a user feedback loop are suggested.
