# 📱 Social Media & Mental Health — Exploratory Data Analysis

A data analysis project exploring the relationship between social media usage and mental health indicators such as anxiety, stress, sleep quality, addiction levels, and academic performance among students.

---

## 📌 Project Overview

This project performs a comprehensive Exploratory Data Analysis (EDA) on a social media and mental health dataset. The goal is to uncover behavioral patterns, identify addiction trends, and understand how social media usage affects students' academic and psychological well-being.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core programming language |
| Pandas | Data loading, cleaning, and analysis |
| NumPy | Feature engineering and numeric operations |
| Matplotlib | Data visualization |
| Jupyter Notebook | Interactive development environment |

---

## 📂 Project Structure

```
Social_Media_EDA/
│
├── Social_Media.ipynb    # Main analysis notebook
├── social.csv            # Dataset (required to run)
└── README.md             # Project documentation
```

---

## 🔍 Analysis Workflow

### 1. 📦 Data Loading
- Loaded dataset from `social.csv`
- Previewed shape, columns, data types, and statistical summary

### 2. 🧹 Data Cleaning
- Checked for missing values
- Filled nulls with 0
- Removed duplicate rows

### 3. ⚙️ Feature Engineering
Created 6 new categorical columns using `np.where`:

| Column | Categories |
|--------|-----------|
| `usage_category` | Low User (0–2h), Medium User (3–5h), Heavy User (>5h) |
| `sleep_category` | Poor Sleep (<5h), Normal Sleep (5–7h), Healthy Sleep (≥8h) |
| `academic_category` | Weak (<2.5), Average (2.5–3.5), Excellent (>3.5) |
| `anxiety_category` | Low Risk (<4), Medium Risk (4–7), High Risk (>7) |
| `stress_category` | Low Risk (<4), Medium Risk (4–7), High Risk (>7) |
| `addiction_category` | Low Risk (<4), Medium Risk (4–7), High Risk (>7) |

### 4. 🔎 Filtering
- Heavy social media users
- High anxiety students
- Poor sleep students
- Weak academic performers

### 5. 📊 GroupBy Analysis
- Average stress level by gender
- Average addiction level by platform
- Academic performance by platform
- Depression count by gender

### 6. 🏆 Top / Bottom Analysis
- Most addicted students
- Students with least sleep
- Highest anxiety levels
- Best academic performers

### 7. 📈 Visualizations
- **Bar Charts** — Gender vs Stress, Platform vs Addiction
- **Line Plot** — Sleep vs Anxiety Trend
- **Histograms** — Social media usage distribution, Anxiety score distribution
- **Scatter Plots** — Social media hours vs Academic performance, Sleep vs Stress
- **Pie Chart** — Usage category distribution
- **Subplots Dashboard** — All 8 charts in a single combined view

---

## 📊 Key Insights

- Heavy social media users tend to report higher anxiety and stress levels
- Poor sleep is associated with increased anxiety scores
- Platform type influences addiction level among students
- Gender-based differences exist in stress and depression indicators

---

## ▶️ How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/priyanshupatel-tech/social-media-eda.git
   cd social-media-eda
   ```

2. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib jupyter
   ```

3. Add the dataset file `social.csv` to the project folder.

4. Launch Jupyter Notebook:
   ```bash
   jupyter notebook Social_Media.ipynb
   ```

---

## 📁 Dataset

The dataset (`social.csv`) includes the following key columns:

- `daily_social_media_hours` — Daily time spent on social media
- `sleep_hours` — Average sleep hours per night
- `anxiety_level` — Self-reported anxiety score (0–10)
- `stress_level` — Self-reported stress score (0–10)
- `addiction_level` — Social media addiction score (0–10)
- `academic_performance` — GPA or equivalent score
- `gender` — Student gender
- `platform_usage` — Primary social media platform used
- `depression_label` — Depression indicator

> **Note:** The dataset file is not included in this repository. You can use your own dataset with the same column structure.

---

## 👤 Author

**[Priyanshu Patel]**
- GitHub: [priyanshupatel-tech](https://github.com/priyanshupatel-tech)
- LinkedIn: [priyanshupatel-tech](https://linkedin.com/in/priyanshupatel-tech)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
