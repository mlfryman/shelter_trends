# 🐾 Cat Shelter Data Insights: Length of Stay & Adoption Analysis

## 📘 Overview

This project explores real shelter operations data exported from **Shelterluv**, focusing on understanding factors that influence cat **length of stay** and **adoption outcomes**.

Using **Python-based data analytics and visualization**, the notebook demonstrates how raw operational data can be transformed into actionable insights for decision-making and performance optimization in animal welfare organizations.

---

## 🎯 Objectives

- Clean and merge Shelterluv demographic and outcome datasets.  
- Calculate **Length of Stay (LOS)** per cat.  
- Identify **adoption patterns and trends** over time.  
- Analyze LOS by demographic factors (**age**, **intake type**, **outcome type**).  
- Build a **predictive model** to estimate LOS and interpret **feature importance**.  

---

## 🧮 Tools & Technologies

| Category | Tools |
|-----------|--------|
| **Language** | Python 3.11+ |
| **Data Analysis** | pandas, numpy |
| **Visualization** | seaborn, matplotlib |
| **Modeling** | scikit-learn |
| **Environment** | Jupyter Notebook |
| **Data Source** | Shelterluv CSV Exports |

---

## 📊 Key Analyses & Results

### 1. Data Preparation
Cleaned and merged two datasets:  
- `SL_data_20251112.csv` (demographics)  
- `SL_length_of_stay_20251112.csv` (outcomes)

Standardized date formats and created a new **Length of Stay (days)** column.  
Extracted **foster names** using regular expressions (e.g., “Foster: Jane Doe”).  

---

### 2. Exploratory Analysis

- **Adoptions by Month:** Bar chart of monthly adoption counts.  
- **Length of Stay Distribution:** Histogram showing typical vs. long-term residents.  
- **Average LOS by Age Group:** Bar chart comparing average stays by age.  

---

### 3. Predictive Modeling

- Implemented a **Random Forest (non-linear regression) model** to predict LOS.  
- Evaluated using:
  - **Mean Absolute Error (MAE):** ~50 days 
  - **R² Score:** 0.11  
- Generated a **feature importance visualization** to identify top predictive factors.

---

## 📈 Example Visuals

- Frequency of Adoptions by Month  
- Average LOS by Age Group
- Distribution of Length of Stay (days)  
- Feature Importance from Predictive Model  

*(All visualizations generated directly in the notebook using seaborn and matplotlib.)*

---

## 📂 Project Structure

shelter_trends/
├── data/
│ ├── SL_data_20251112.csv
│ ├── SL_length_of_stay_20251112.csv
├── notebooks/
│ └── shelter_data_analysis.ipynb
├── README.md
└── requirements.txt

---

## 🚀 How to Run

### 1. Clone the repository:
```bash
git clone https://github.com/<your-username>/shelter_trends.git
cd shelter_trends
```

### 2. Create a virtual environment & install dependencies:
```bash
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows
pip install -r requirements.txt
```

### 3. Open the Notebook
```bash
jupyter notebook notebooks/shelter_data_analysis.ipynb
```

### 4. Run all cells to reproduce the full workflow and visualizations.

---

## 💡 Future Work

- Add more features (e.g., color, foster, season, adoption fee group).
- Explore seasonality and event-driven adoption patterns.
- Integrate Shelterluv API for automated data updates.
- Create web app via Streamlit
---

## 🧑‍💻 Author

**[Bash Melanie Fryman]** — Data Analyst / Software Developer  
📫 [bmlf72@gmail.com]  
💻 [github.com/mlfryman]

---

## 📄 License

This project is released under **The Unlicense**.  
See the [LICENSE](./LICENSE) for more details.