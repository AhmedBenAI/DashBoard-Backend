# 📊 Automated Dashboard Backend (Flask AppBuilder)

An intelligent backend system built with **Flask-AppBuilder** for dynamic and automated dashboard generation using **machine learning** techniques.

This project was developed as part of my MSc research at **USTOMB (Oran, Algeria)**, focusing on the **automation of dashboard creation** by analyzing dataset characteristics, performing feature selection, and recommending the most suitable visualizations.

---

## 💡 Overview

The backend analyzes CSV datasets, applies data preprocessing and feature importance algorithms, and dynamically selects chart types that best represent the data.

The generated outputs are served via a simple REST API, which can be consumed by a separate frontend for visualization.

---

## 🧠 Key Features

- 📂 **Dataset Management:** Automatically detects and lists available CSV datasets.  
- 📈 **ML-Driven Chart Selection:** Uses feature importance and data properties to recommend chart types.  
- 🧮 **Automated Dashboard Generation:** Dynamically generates visualizations for a given dataset.  
- 🔗 **RESTful API Endpoints:** Provides a clean and easy interface for frontend integration.  

---

## ⚙️ Tech Stack

**Framework:** Flask-AppBuilder (Flask)  
**Languages:** Python  
**Libraries:** Pandas · NumPy · Scikit-Learn · Matplotlib / Plotly  
**Environment:** Python 3.x  

---

## 🚀 Setup Instructions

### 1️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 2️⃣ Run the API Server

```bash
cd AutoChartBackend
python api.py
```

Server will start on port **5000**.

---

## 🔗 API Endpoints

| Endpoint | Description |
|-----------|-------------|
| `/datasets` | Returns a list of all available CSV datasets in the `data` folder |
| `/chart/<string:chart>` | Returns the selected main and secondary chart types recommended by the ML model |
| `/htmlread/<string:file>` | Returns the HTML file for rendering on the frontend |

---

## 🧩 Example Workflow

1. Upload or store your dataset in the `data/` folder.  
2. Call the `/datasets` endpoint to list all available data sources.  
3. Select a dataset — the system analyzes features and recommends charts.  
4. The `/htmlread/<file>` endpoint serves the corresponding HTML visualization.

---

## 🧪 Research Context

This backend was created as part of my MSc research project at **USTOMB (Oran, Algeria)**.  
The work focused on:
- Automating dashboard generation using **machine learning**.
- Applying **feature importance** and **data cleaning** techniques to determine relevant data features.
- Selecting the most informative chart types for presentation.

🧾 The full dissertation accompanying this project provides detailed methodology and results.

---

## 📚 Future Improvements

- ⏳ Integrate FastAPI for performance optimization.  
- ⏳ Add user authentication and dataset upload endpoints.  
- ⏳ Develop a React/Angular-based frontend for interactive dashboards.  

---

## 👤 Author

**Ahmed Bendimered**  
🎓 MSc in Artificial Intelligence — USTOMB, Oran  
🎓 MSc in Artificial Intelligence (Applied Machine Learning) — Liverpool John Moores University  
🔗 [LinkedIn](https://www.linkedin.com/in/bendimered-ahmed-el-hadi)  
📍 Liverpool, UK · Open to relocation or remote opportunities  

---

> *An AI-driven approach to automating data visualization and dashboard generation.*
