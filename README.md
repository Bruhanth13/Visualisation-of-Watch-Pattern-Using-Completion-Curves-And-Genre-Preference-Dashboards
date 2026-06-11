# 📺 Visualisation of Watch Patterns Using Completion Curves and Genre Preference Dashboards

> A data analysis and visualisation project exploring how streaming platform users consume content — uncovering watch completion behaviour, genre preferences, device usage, and engagement trends through interactive dashboards.

---

## 📌 Project Overview

This project analyses a real-world-style streaming dataset of **5,000 watch sessions** across 6 regions and 8 genres. The aim is to transform raw watch history data into meaningful visual stories using completion curves and a genre preference dashboard.

**Two core questions answered:**
- **How far do viewers actually watch?** — Using completion curves and a funnel chart to track drop-off stages.
- **What do viewers prefer and when?** — Using an interactive multi-panel dashboard showing genre watch time, device usage, subscription share, and streaming trends over time.

---

## 📁 Project Files

```
watch-pattern-analysis/
│
├── Watch_patterns_dataset.csv              # Dataset — 5,000 watch session records
└── Watch_Pattern_Analysis_.ipynb           # Full analysis notebook (loading → conclusion)
```

---

## 📊 Dataset

The dataset contains **5,000 rows** and **15 columns** covering viewer watch sessions on a streaming platform.

| Column | Description |
|--------|-------------|
| `user_id` | Unique viewer identifier |
| `content_id` | Unique content identifier |
| `content_title` | Name of the show or movie |
| `genre` | Content genre (Comedy, Drama, Action, Thriller, Sci-Fi, Romance, Animation, Documentary) |
| `total_duration_min` | Full content length in minutes |
| `watched_duration_min` | Minutes actually watched by the user |
| `completion_rate_percent` | Percentage of content completed |
| `watch_session_length_min` | Duration of the viewing session in minutes |
| `device_type` | Device used (Mobile, Laptop, Tablet, Smart TV) |
| `subscription_type` | User plan (Free, Basic, Standard, Premium) |
| `watch_date` | Date of the watch session |
| `watch_start_hour` | Hour of the day when viewing started (0–23) |
| `region` | Viewer's region (India, USA, UK, Germany, Canada, Australia) |
| `rating_given` | User rating (1–5) |
| `rewatch_flag` | 1 = rewatch, 0 = first watch |

---

## 🛠️ Tech Stack

| Library | Purpose |
|---------|---------|
| Python 3.x | Core language |
| Pandas | Data loading, cleaning, exploration |
| NumPy | Numerical operations |
| Plotly Express | Interactive charts (bar, scatter, pie, histogram, line) |
| Plotly Graph Objects | Funnel chart, animated scatter, 3D plot, dashboard |
| Jupyter Notebook | Development and presentation environment |

---

## 📈 Visualisations Built

### Exploratory Analysis
| Chart | What it shows |
|-------|--------------|
| Bar chart — Genre Distribution | Which genres are watched most frequently |
| Pie chart — Device Usage | Proportion of viewers by device type |
| Scatter plot — Completion Rate vs Rating | Whether higher watch completion leads to better ratings |
| Histogram — Watch Start Hour | Peak hours when viewers start watching |
| Bar chart — Region Wise Viewers | Which regions contribute most viewing sessions |
| Pie chart — Rewatch vs First Watch | How many viewers rewatch content |
| Box plot — Subscription Type vs Rating | How ratings vary across Free, Basic, Standard, Premium plans |
| Sunburst chart — Viewing Hierarchy | Genre → Device → Subscription breakdown in one chart |

### Core Deliverables
| Chart | What it shows |
|-------|--------------|
| **Funnel chart — Viewer Completion Funnel** | Drop-off from Started → Half Completed → Fully Completed |
| **Animated scatter — Watching Behaviour Over Time** | How genre engagement and completion evolve day by day |
| **Animated scatter — Device Usage Evolution** | How device preferences shift over time |
| **3D scatter — Viewing Behaviour Analysis** | Watch duration, completion rate, and session length across genres |
| **Bubble plot — Genre Rating Analysis** | Genre vs rating with completion rate as bubble size |
| **Genre Preference Dashboard** | Full multi-panel dashboard: KPIs + trend + genre + device + subscription |

---

## 🔍 Key Findings

- **5,000** total watch sessions analysed across **3,860** unique active users
- Total watch time: **253,300+ minutes** with an average completion rate of **50.7%**
- **Drop-off is steep** — of 5,000 viewers who started content, only 2,510 watched beyond 50% and just 505 completed it fully
- **Mobile** is the dominant viewing device across the platform
- **Subscription type influences ratings** — Premium users tend to give higher and more consistent ratings compared to Free/Basic users
- Ratings are fairly distributed across genres, but completion rates vary, suggesting content quality affects engagement more than genre alone

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/Bruhanth13/Visualisation-of-Watch-Pattern-Using-Completion-Curves-And-Genre-Preference-Dashboards
cd watch-pattern-analysis
```

### 2. Install dependencies
```bash
pip install pandas numpy plotly jupyter
```

### 3. Open the notebook
```bash
jupyter notebook Watch_Pattern_Analysis_.ipynb
```

### 4. Make sure the dataset is in the same folder as the notebook
The notebook loads the CSV with:
```python
df = pd.read_csv("Watch_patterns_dataset.csv")
```

---

## 👥 Authors

**Group Name:Visualisation of Watch Patterns

| Name | GitHub | LinkedIn |
|------|--------|----------|
| Member 1 M.Bruhanth       | [@username](https://github.com/username) | [linkedin](https://linkedin.com/in/username) |
| Member 2 B.Kasturi        | [@username](https://github.com/username) | [linkedin](https://linkedin.com/in/username) |
| Member 3 P.Harsha vardhan | [@username](https://github.com/username) | [linkedin](https://linkedin.com/in/username) |
| Member 4 G.Harshitha      | [@username](https://github.com/username) | [linkedin](https://linkedin.com/in/username) |

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
---

This project is open source and available under the [MIT License](LICENSE).
