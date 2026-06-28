# 📊 Google Play Store Category Growth Analysis Dashboard

> A Data Analytics and Visualization project that analyzes cumulative app installation trends across Google Play Store categories and highlights high-growth periods using Python and Matplotlib.

---

# 📑 Table of Contents

- <a href="#project-title">Project Title</a>
- <a href="#brief-summary">Brief One Line Summary</a>
- <a href="#overview">Overview</a>
- <a href="#problem-statement">Problem Statement</a>
- <a href="#dataset">Dataset</a>
- <a href="#tools-and-technologies">Tools and Technologies</a>
- <a href="#methods">Methods</a>
- <a href="#key-insights">Key Insights</a>
- <a href="#dashboard-model-output">Dashboard / Output</a>
- <a href="#project-structure">Project Structure</a>
- <a href="#how-to-run-this-project">How to Run this Project?</a>
- <a href="#results-conclusion">Results & Conclusion</a>
- <a href="#future-work">Future Work</a>
- <a href="#author-contact">Author & Contact</a>

---

<h2 id="project-title">📌 Project Title</h2>

# Google Play Store Category Growth Analysis Dashboard

---

<h2 id="brief-summary">📝 Brief One Line Summary</h2>

A Python-based data analytics dashboard that visualizes cumulative app installation trends across Google Play Store categories and identifies significant growth periods using stacked area charts.

---

<h2 id="overview">📖 Overview</h2>

This project analyzes Google Play Store application data to understand how different app categories grow over time based on installation counts.

The system cleans and preprocesses app data, applies business-driven filtering rules, aggregates installation trends monthly, calculates growth rates, and visualizes category performance using an interactive stacked area chart.

Special emphasis is placed on identifying months where categories experience significant growth, helping uncover trends and market opportunities.

---

<h2 id="problem-statement">⚠️ Problem Statement</h2>

With thousands of applications across multiple categories, identifying which categories are experiencing rapid growth can be difficult.

This project aims to:

- Analyze installation growth trends over time
- Compare category-wise app performance
- Identify high-growth periods
- Visualize cumulative installs
- Support business intelligence and market analysis
- Discover emerging app categories

---

<h2 id="dataset">📂 Dataset</h2>

The project uses Google Play Store application data containing:

### Dataset Features

- App Name
- Category
- Rating
- Reviews
- Installs
- Size
- Last Updated

### Data Cleaning Performed

- Rating conversion to numeric format
- Review count cleaning
- Installation count cleaning
- App size standardization
- Date conversion
- Missing value handling

---

<h2 id="tools-and-technologies">🛠️ Tools and Technologies</h2>

## Programming Language

- Python

## Libraries Used

- Pandas
- NumPy
- Matplotlib
- PyTZ
- Datetime
- Regular Expressions (re)

## Development Environment

- Jupyter Notebook
- VS Code

---

<h2 id="methods">⚙️ Methods</h2>

## 1. Data Cleaning

Performed preprocessing on:

- Ratings
- Reviews
- Installs
- App Size
- Last Updated Date

### Installation Cleaning

```text
10,000+ → 10000
1,000,000+ → 1000000
```

---

## 2. Business Rule Filtering

Applications were filtered using:

### Rating Filter

```text
Rating ≥ 4.2
```

### Reviews Filter

```text
Reviews > 1000
```

### App Size Filter

```text
20 MB ≤ Size ≤ 80 MB
```

### Category Filter

Only categories beginning with:

```text
T and P
```

Examples:

- Travel & Local
- Productivity
- Photography

### App Name Filter

Applications containing numerical digits were excluded.

---

## 3. Monthly Aggregation

The project aggregates installation counts based on:

- Month
- Category

Monthly cumulative installations are calculated to analyze long-term trends.

---

## 4. Category Translation

Category names are translated for dashboard presentation:

| Original Category | Dashboard Label |
|------------------|----------------|
| Travel & Local | Voyages et Local |
| Productivity | Productividad |
| Photography | 写真 |

---

## 5. Growth Analysis

Month-over-month growth rates are calculated using:

```text
Growth Rate = (Current Month - Previous Month)
/ Previous Month
```

Categories experiencing:

```text
Growth > 25%
```

are automatically highlighted.

---

## 6. Visualization

A stacked area chart is generated to display:

- Category-wise cumulative installs
- Growth patterns
- Category comparison
- High-growth periods

---

<h2 id="key-insights">📊 Key Insights</h2>

- Productivity and Photography applications show strong install growth.
- Installation trends reveal seasonal growth patterns.
- Certain months experience significantly higher growth than others.
- Category-wise aggregation provides clearer market insights.
- Growth detection helps identify emerging opportunities.

---

<h2 id="dashboard-model-output">📈 Dashboard / Output</h2>

## Dashboard Workflow

```text
Google Play Store Dataset
          ↓
Data Cleaning
          ↓
Business Rule Filtering
          ↓
Monthly Aggregation
          ↓
Category Translation
          ↓
Growth Calculation
          ↓
Highlight Significant Months
          ↓
Stacked Area Chart Visualization
```

---

## 📊 Visualization Generated

### Stacked Area Chart

Displays:

- Category-wise cumulative installs
- Monthly install trends
- Category contribution comparison

### Growth Highlighting

Months with:

```text
Growth > 25%
```

are highlighted using shaded regions.

### Time Awareness

Dashboard includes IST timezone handling using:

```python
Asia/Kolkata
```

for time-based monitoring.

---

<h2 id="project-structure">📁 Project Structure</h2>

```bash
Google_Play_Store_Growth_Analysis/

│
├── task4.ipynb
├── google_play_store_dataset.csv
├── README.md
└── outputs/
```

---

<h2 id="how-to-run-this-project">🚀 How to Run this Project?</h2>

## Clone Repository

```bash
git clone https://github.com/yashrajmohanty03-ai/google-play-store-growth-analysis.git

cd google-play-store-growth-analysis
```

## Install Dependencies

```bash
pip install pandas numpy matplotlib pytz
```

## Run Notebook

```bash
jupyter notebook task4.ipynb
```

## Execute All Cells

Run all notebook cells sequentially to:

- Load dataset
- Clean data
- Apply filtering rules
- Aggregate installs
- Calculate growth rates
- Generate stacked area chart

---

<h2 id="results-conclusion">📈 Results & Conclusion</h2>

## Results

The dashboard successfully:

- Cleaned and transformed Play Store data
- Applied business-driven filtering criteria
- Aggregated category-wise installs
- Calculated month-over-month growth
- Identified significant growth periods
- Generated a stacked area visualization highlighting trends

---
## Output
![image alt](https://github.com/yashrajmohanty03-ai/Ev4/blob/0b5d30079abb6e28cdc7ec391afa0833bb0b7b99/op%204.png)

## Conclusion

This project demonstrates how data analytics and visualization techniques can uncover meaningful growth trends within the Google Play Store ecosystem. By combining category filtering, cumulative installation analysis, and growth detection, the dashboard provides actionable insights for market research and business intelligence.

---

<h2 id="future-work">🔮 Future Work</h2>

Future enhancements include:

- Interactive Plotly dashboards
- Streamlit deployment
- Real-time Play Store integration
- Predictive growth forecasting
- Category recommendation system
- Power BI integration
- Advanced business intelligence reporting

---

<h2 id="author-contact">👨‍💻 Author & Contact</h2>

## Yashraj Mohanty

### Areas of Interest

- Data Analytics
- Data Visualization
- Business Intelligence
- Machine Learning

### Contact

- GitHub: https://github.com/yashrajmohanty03-ai
- LinkedIn: https:// linkedin.com/in/yashraj-mohanty
- Email: yashrajmohanty3@gmail.com

---

<p align="center">
⭐ If you found this project useful, consider giving it a star on GitHub!
</p>
