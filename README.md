# 🌾 Crop Yield Predictor

A web app that predicts expected crop yield based on field conditions — rainfall, temperature, fertilizer usage, and cultivated area — using a trained Random Forest Regressor. Built with Streamlit.

## What it does

Enter a field's rainfall, temperature, fertilizer usage, and area, and the app predicts:
- Expected yield in tons per hectare
- Estimated total output for the area entered

It also shows which input factors matter most to the model's predictions.

## Demo

*(screenshot/screen recording here)*

## Model

- **Algorithm:** Random Forest Regressor (100 estimators)
- **Features:** Rainfall, Temperature, Fertilizer, Area
- **Target:** Yield (tons/hectare)
- **Performance:** R² score ≈ 0.90, mean absolute error ≈ 0.27 tons/hectare
- **Dataset:** 300 field records

## Run it locally

```bash
pip install streamlit pandas scikit-learn
streamlit run app.py
```

Then open `http://localhost:8501` in your browser.

## Tech stack

- Python
- Streamlit — UI and web app framework
- scikit-learn — model training and inference
- pandas — data handling

## Disclaimer

This is an educational project. Predictions are illustrative and shouldn't be used as the sole basis for real agricultural planning decisions.
