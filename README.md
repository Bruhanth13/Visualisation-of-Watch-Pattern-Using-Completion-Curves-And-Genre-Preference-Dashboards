# 📺 Visualisation of Watch Patterns Using Completion Curves and Genre Preference Dashboards

> An end-to-end data analysis and visualisation project that explores how viewers consume content — uncovering watch completion behaviour and genre preference trends through interactive dashboards.

---

## 📌 Project Overview

This project analyses streaming watch data to answer two core questions:

- **How far do viewers watch?** — Using *completion curves* to visualise drop-off patterns across episodes or runtimes.
- **What do viewers prefer?** — Using *genre preference dashboards* to map taste distribution across demographics, time, or platforms.

The goal is to transform raw watch history data into meaningful visual stories that can guide content recommendations, production decisions, or user experience improvements.

---

## 🎯 Key Features

- 📈 **Completion Curve Analysis** — Line/area charts showing the percentage of viewers who complete a show at each time interval (episode 1 → finale).
- 🎭 **Genre Preference Dashboard** — Bar charts, pie/donut charts, and heatmaps showing which genres dominate watch time by user segment.
- 🔍 **Drop-off Detection** — Identifies episodes or timestamps where viewer retention falls sharply.
- 📊 **Interactive Visualisations** — Built with Matplotlib & Seaborn (or Plotly for interactivity).
- 🧹 **Data Cleaning Pipeline** — Handles missing values, duplicates, and inconsistent formatting in raw watch data.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.x | Core language |
| Pandas | Data loading, cleaning, transformation |
| NumPy | Numerical operations |
| Matplotlib | Static charts (completion curves) |
| Seaborn | Styled statistical plots |
| Plotly *(optional)* | Interactive dashboards |
| Jupyter Notebook | Development & presentation |

---

## 📁 Project Structure

```
watch-pattern-analysis/
│
├── data/
│   ├── raw/                    # Original dataset (CSV/JSON)
│   └── cleaned/                # Processed data files
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb          # Data preprocessing steps
│   ├── 02_completion_curves.ipynb      # Watch completion analysis
│   └── 03_genre_dashboard.ipynb        # Genre preference visualisations
│
├── outputs/
│   ├── completion_curve.png            # Exported chart images
│   └── genre_dashboard.png
│
├── src/
│   ├── data_loader.py          # Functions to load & clean data
│   ├── completion_analysis.py  # Logic for completion curve generation
│   └── genre_analysis.py       # Logic for genre preference analysis
│
├── requirements.txt
└── README.md
```

---

## 📊 Dataset

The dataset contains streaming watch records with the following fields:

| Column | Description |
|--------|-------------|
| `user_id` | Unique viewer identifier |
| `show_title` | Name of the series or movie |
| `genre` | Category (Drama, Comedy, Thriller, etc.) |
| `episode_number` | Episode watched (for series) |
| `watch_duration_min` | Minutes watched in a session |
| `total_duration_min` | Full content length |
| `completion_%` | Percentage of content completed |
| `watch_date` | Date of the watch session |

> **Note:** Data was either synthetically generated for practice or sourced from a public dataset (e.g., Netflix Prize dataset, MovieLens).

---

## 📉 Completion Curves — What They Show

A completion curve plots the **percentage of viewers who reach each point** in a show.

```
100% |████████████████
 85% |         ████████████
 60% |                  ████████
 40% |                           ████
 20% |                                ████
      Ep1   Ep2   Ep3   Ep4   Ep5   Ep6   Finale
```

- A **steep early drop** means viewers abandon shows after the first episode.
- A **gradual decline** is normal — it shows sustained but decreasing engagement.
- A **spike at the finale** means viewers who stayed are highly committed.

---

## 🎭 Genre Preference Dashboard — What It Shows

The genre dashboard answers:
- Which genres have the **highest average completion rate**?
- Which genres are watched the **most frequently** per user?
- How do preferences shift **over time** (monthly/seasonally)?

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/watch-pattern-analysis.git
cd watch-pattern-analysis
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Open Jupyter Notebook
```bash
jupyter notebook
```

### 4. Run notebooks in order
```
01_data_cleaning.ipynb  →  02_completion_curves.ipynb  →  03_genre_dashboard.ipynb
```

---

## 📸 Sample Visualisations

> *(Add your chart screenshots here once generated)*

| Completion Curve | Genre Dashboard |
|-----------------|----------------|
| ![completion](outputs/completion_curve.png) | ![genre](outputs/genre_dashboard.png) |

---

## 💡 Key Insights (Example)

- **Drama** has the highest average completion rate (78%), followed by **Documentary** (72%).
- Most drop-offs occur between **Episode 2 and Episode 3** — a critical retention window.
- **Thriller** genre sees a spike in watch time during **weekend evenings**.
- Users who watch 3+ genres have a **40% higher** overall completion rate.

> *(Replace these with your actual findings after running the analysis)*

---

## 🔮 Future Improvements

- [ ] Add user segmentation (age group, region) to genre analysis
- [ ] Build a Plotly Dash or Streamlit interactive web dashboard
- [ ] Incorporate recommendation engine based on completion patterns
- [ ] Add time-series analysis for seasonal watch trends

---

## 👤 Author

**Your Name**
- GitHub: [@yourusername](https://github.com/yourusername)
- LinkedIn: [linkedin.com/in/yourprofile](https://linkedin.com/in/yourprofile)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
