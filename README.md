# 🎬 Cinematic Data Dive | Netflix Movies & Shows Analysis

### 📊 Power BI | Power Query | DAX | Data Analytics | Data Visualization

## 📌 Project Overview

**Cinematic Data Dive** is a data analytics project focused on exploring Netflix movies and TV shows using **Microsoft Power BI**.

The project analyzes **5,283 titles spanning 70 years (1953–2022)** to identify trends in content distribution, IMDb ratings, audience engagement, runtime, and age certifications.

The objective is to transform raw entertainment data into meaningful visual insights that can support **content acquisition, production strategies, and data-driven business decisions**.

---

## 🎯 Project Objectives

- Analyze the distribution of movies and TV shows across different release years.
- Examine IMDb ratings and audience engagement using IMDb vote counts.
- Identify patterns between content runtime and audience ratings.
- Explore content distribution across different age certification categories.
- Develop interactive dashboards to communicate insights effectively.
- Enable dynamic data exploration through filters and slicers.

---

## 📂 Dataset Information

**Dataset:** Netflix Movies & Shows (IMDb Data)

**Total Records:** 5,283

**Time Period:** 1953–2022

### Key Attributes

| Column | Description |
|--------|-------------|
| `id` | Unique identifier for each title |
| `title` | Name of the movie or TV show |
| `type` | Content type (Movie/Show) |
| `release_year` | Year of release |
| `runtime` | Duration in minutes |
| `imdb_score` | IMDb rating |
| `imdb_votes` | Number of IMDb votes |
| `age_certification` | Age-based content classification |
| `description` | Description of the content |

---

## 🛠️ Tools & Technologies

| Technology | Usage |
|------------|-------|
| **Power BI** | Interactive dashboards and data visualization |
| **Power Query** | Data cleaning and transformation |
| **DAX** | Calculated columns and analytical calculations |
| **Data Modeling** | Organizing data for analysis |
| **Data Visualization** | Communicating trends and patterns |

---

## 🔄 Data Preparation & Transformation

The dataset was imported into **Power BI Desktop** using Power Query Editor.

### Key Transformation Tasks

**1. Rating × Votes**

Created a calculated column to combine IMDb ratings and vote counts.

```powerquery
[imdb_score] * [imdb_votes]
```

**2. Runtime Conversion**

Converted runtime from minutes into hours using DAX.

```dax
runtime_hrs = 'Netflix'[runtime] / 60
```

*Note: Replace `Netflix` with the actual table name in your Power BI model.*

**3. Data Quality**

- Reviewed missing values in age certification.
- Examined runtime values and their distribution.
- Applied appropriate filtering and transformations.
- Prepared the dataset for interactive reporting.

---

## 📊 Dashboard Features

The Power BI dashboard contains multiple interactive visualizations.

### 🎥 1. Movies & TV Shows Distribution

- Donut chart displaying movies released across different years.
- Pie chart representing TV shows released annually.
- Focused analysis on content released after 2010.

### ⭐ 2. IMDb Ratings & Audience Engagement

- Analyzed IMDb ratings and vote counts.
- Examined the relationship between runtime and rating-weighted votes.
- Visualized variations in audience engagement.

### 🔞 3. Age Certification Analysis

- Bar chart displaying the distribution of movies by age certification since 2000.
- Compared rating-weighted votes across age certification categories.
- Examined average runtime across different content classifications.

### 🎛️ 4. Interactive Filters

The dashboard includes slicers for:

- **Release Year:** Filter content by release year.
- **Runtime:** Select a duration range.
- **Content Type:** Switch between movies and shows.

These filters allow users to explore different segments of the dataset.

---

## 📈 Analysis Highlights

The dashboard enables users to investigate:

- Changes in movie and TV show releases over time.
- Distribution of content across age certification categories.
- Relationships between content duration and audience engagement.
- Differences in rating-weighted votes across content categories.
- Content trends relevant to entertainment analytics.

---

## 📸 Dashboard Preview

Add a screenshot of your Power BI dashboard here.

```markdown
![Netflix Power BI Dashboard](images/dashboard.png)
```

Create an `images` folder in your repository and upload your dashboard screenshot as `dashboard.png`.

---

## 📁 Repository Structure

```text
Cinematic-Data-Dive/
│
├── README.md
│
├── dataset/
│   └── netflix_titles.csv
│
├── dashboard/
│   └── Cinematic_Data_Dive.pbix
│
└── images/
    └── dashboard.png
```

*This is a suggested structure. Update file names and paths to match your repository.*

---

## 🚀 How to Use

1. Clone or download this repository.
2. Install **Microsoft Power BI Desktop**.
3. Open the `.pbix` file from the `dashboard` folder.
4. Refresh the dataset if required.
5. Explore the dashboard using interactive filters and visualizations.

---

## 💡 Business Applications

The analysis can support entertainment and OTT platforms in:

- **Content Strategy:** Understanding historical release patterns.
- **Audience Engagement:** Exploring IMDb rating and voting trends.
- **Content Classification:** Examining age-based content distribution.
- **Programming Decisions:** Understanding runtime patterns across content categories.
- **Business Intelligence:** Presenting entertainment data through interactive dashboards.

---

## 🎓 Skills Demonstrated

`Power BI` `Power Query` `DAX` `Data Cleaning` `Data Transformation` `Exploratory Data Analysis` `Data Visualization` `Dashboard Development` `Business Intelligence`

---

## 👨‍💻 Author

**Arpit Singh**

*Data Analyst | SQL | Python | Power BI | Excel*

---

### ⭐ If you find this project useful, consider giving the repository a star!
