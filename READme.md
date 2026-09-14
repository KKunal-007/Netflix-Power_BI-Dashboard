# 🎬 Netflix Content Analysis Dashboard (Power BI)

An interactive Power BI dashboard analyzing Netflix's global content catalog — titles, cast, directors, genres, and release patterns by country.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/status-complete-brightgreen)

## 📊 Overview

This dashboard explores Netflix's content library to surface trends in what gets released, where, and by whom. It's built on a relational data model with six connected tables rather than a single flat file, so the report can slice content by country, genre, cast, and director independently.

## 🗂️ Data Model

| Table | Description |
|---|---|
| `netflix_titles` | Core fact table — one row per title (movie/show), with type, date added, rating, duration, etc. |
| `countries_released` | Country-level release data (bridge table for titles released in multiple countries) |
| `netflix_listed_in` | Genre/category tags per title |
| `netflix_cast` | Cast members per title |
| `netflix_directors` | Director(s) per title |
| `description` | Title descriptions/synopses |

## 📄 Report Pages

- **Overview Page** — Area chart of content added over time, column chart and clustered bar chart breakdowns (e.g., by genre/type), and a world map of releases by country.
- **Details Page** — Drill-down view with KPI cards, country/genre/type slicers, a filterable map, and a detailed data table.

## 🛠️ Tools Used

- Power BI Desktop
- Power Query for data shaping
- DAX for calculated measures

## 🚀 How to Use

1. Download `Netflix_Dataset.pbix`.
2. Open it in [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free).
3. Use the slicers on the Details page to filter by country, genre, or content type.

> **Note:** GitHub can preview `.pbix` files as a download only — it won't render the report inline. Add a screenshot or GIF below so visitors can see the dashboard without opening Power BI.

## 📸 Preview

<img width="1237" height="743" alt="Screenshot 2026-09-14 073145" src="https://github.com/user-attachments/assets/ba54ac09-703f-46d6-b5d8-bef0099ce32b" />

<img width="1237" height="741" alt="Screenshot 2026-09-14 073044" src="https://github.com/user-attachments/assets/51c58d76-ac05-4203-a85b-e0153442bb50" />


## 📁 Data Source

Netflix titles dataset (commonly sourced from the public [Netflix Movies and TV Shows dataset on Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows)).

## 👤 Author

[Kunal](https://github.com/KKunal-007)
