# Spotify

# 🎧 Spotify Top 50 World – Power BI Dashboard

A Spotify-inspired **Power BI analytics dashboard** that visualizes the **Top 50 songs worldwide**, focusing on popularity trends, artist performance, explicit content analysis, and song characteristics — all wrapped in a **modern dark UI inspired by Spotify**.

---

## 📌 Project Overview

This project analyzes Spotify’s **Top 50 World Songs** dataset and presents insights using an **interactive Power BI dashboard** designed to visually match Spotify’s user interface.

The dashboard helps answer questions such as:
- Which artists dominate global charts?
- What song attributes influence popularity?
- Do explicit songs perform better?
- How does song duration impact popularity?

---

## 🎯 Key Features

- 🎨 **Spotify-style dark theme UI**
- 📊 KPI Cards for quick insights
- 🎤 Artist & Song performance analysis
- 🔥 Popularity trend tracking
- 🚫 Explicit vs Non-explicit content comparison
- ⏱️ Duration vs Popularity correlation
- 🧠 Advanced DAX measures using a centralized `_Measures` table

---

## 🗂️ Dataset Information

**Source:** Spotify Top 50 World  
**Format:** CSV  
**Records:** Top 50 songs per date  
**File:** `spotify-top-50-world.csv`

### Columns Used
- `date`
- `position`
- `song`
- `artist`
- `popularity`
- `duration_ms`
- `album_type`
- `total_tracks`
- `release_date`
- `is_explicit`
- `album_cover_url`

---

## 🛠️ Tools & Technologies

- **Power BI Desktop**
- **DAX (Data Analysis Expressions)**
- **Power Query**
- **CSV Dataset**
- **UI/UX Design Principles**

---

## 📊 Dashboard Pages

### 🏠 Overview
- Total Songs
- Total Artists
- Total Albums
- Average Popularity
- Highlight KPI (Top Popularity)
- Spotify-style navigation bar

### 🎤 Artists Analysis
- Top Artists by Average Popularity
- Artist contribution to Top 50
- Songs per Artist

### 🎵 Songs Analysis
- Top Songs by Popularity
- Chart Position analysis
- Duration vs Popularity scatter

---

## 🧮 DAX Highlights

- Centralized `_Measures` table
- Aggregations:
  - Total Songs
  - Average Popularity
  - Best/Worst Position
- Time-based insights:
  - Songs per Day
- Content insights:
  - Explicit Song Percentage

Example:
```DAX
Average Popularity = AVERAGE('Top-50-world'[popularity])
