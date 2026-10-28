<div align="center">
🎬 NETFLIX CONTENT ANALYTICS DASHBOARD
An interactive Power BI dashboard exploring what's streaming on Netflix: genres, countries, ratings, audiences & growth over time.

Show Image Show Image Show Image Show Image Show Image

</div>
📸 Dashboard Preview
<div align="center">

Netflix Dashboard

Dark, Netflix-inspired interface with fully interactive slicers and cross-filtering visuals.

</div>
📌 Table of Contents
Overview
Key Features
Dataset
Data Preparation
Dashboard Components
Key Insights
Tech Stack
Project Structure
How to Use
Future Improvements
Author
🎯 Overview

This project turns raw Netflix catalog data into a clean, interactive business-intelligence dashboard built in Microsoft Power BI. It helps answer questions such as:

🎥 How much of the catalog is Movies vs TV Shows?
🌍 Which countries produce the most content?
🎭 Which genres dominate the platform?
👨‍👩‍👧 Which audience groups (Kids, Teens, Adults) are targeted most?
📈 How has content addition changed year over year?
✨ Key Features
Feature	Description
🎛️ Dynamic Slicers	Filter by Type, Release Year, Audience and Director
📊 KPI Cards	Total Titles, Movies and TV Shows at a glance
🍩 Content Split	Donut chart of Movies vs TV Shows
📈 Trend Analysis	Area/line chart of titles by year
🎭 Top 8 Genres	Ranked bar chart of primary genres
🌎 Top 8 Countries	Ranked bar chart of primary countries
⭐ Rating Breakdown	Titles by maturity rating (TV-MA, TV-14, PG-13…)
🎨 Premium UI	Custom dark theme, Netflix-red palette, 3D emblem and logo
📂 Dataset
Source: Netflix Movies and TV Shows – Kaggle
File used: netflix_clean.csv (cleaned & feature-engineered version)
Size: 5,336 titles × 20 columns
Coverage: Content released 1942–2021, added to Netflix 2008–2021
Column	Description
show_id	Unique title ID
type	Movie / TV Show
title, director, cast	Title metadata
country, primary_country	All countries / main production country
date_added, year_added, month_added	When it was added to Netflix
release_year	Original release year
rating	Maturity rating (TV-MA, PG-13, etc.)
duration, duration_value, duration_unit	Raw and split duration (min / Seasons)
listed_in, primary_genre	All genres / main genre
content_age, audience	Derived age of content & audience group (Kids / Teens / Adults)
description	Short synopsis
🧹 Data Preparation

Cleaning and feature engineering were done before loading into Power BI:

✅ Handled missing values in director, cast, country, rating
✅ Converted date_added to a proper date type
✅ Extracted year_added and month_added
✅ Split duration into numeric value and unit
✅ Created primary_genre and primary_country from multi-value columns
✅ Grouped ratings into an audience category
✅ Calculated content_age (years since release)
📊 Dashboard Components
┌──────────────────────────────────────────────────────────────┐
│  NETFLIX                                                     │
├──────────┬──────────────┬───────────┬───────────────────────┤
│  TYPE    │ RELEASE YEAR │ AUDIENCE  │ TOTAL │ MOVIES │ TV   │
│ (slicer) │  (slider)    │ DIRECTOR  │ TITLES│        │SHOWS │
├──────────┴──────────────┴───────────┴───────────────────────┤
│  Movies vs TV Shows  │      Count of Titles by Year         │
├──────────────────────┼──────────────────┬───────────────────┤
│   Top 8 Genres       │  Top 8 Countries │  Titles by Rating │
└──────────────────────┴──────────────────┴───────────────────┘
💡 Key Insights
🎬 Movies dominate the catalog: ~97% of titles are Movies vs ~3% TV Shows in this dataset.
🎭 Dramas (1,519) and Comedies (1,127) are the leading primary genres, followed by Action & Adventure (806).
🌍 The United States (2,133) leads production, followed by India (910) and the United Kingdom (347).
👥 Adults (2,602) and Teens (2,390) make up the bulk of the audience; Kids content is only ~5%.
📈 Content additions peaked in 2019 (1,265 titles), with strong years in 2018 and 2020.
🔞 TV-MA and TV-14 are the most common maturity ratings.

📝 Insights reflect the cleaned dataset, which is skewed toward movies.

🛠️ Tech Stack
Tool	Purpose
Power BI Desktop	Dashboard design & visualization
DAX	Measures and calculated columns
Power Query	Data transformation
Python (Pandas)	Data cleaning & feature engineering
Kaggle	Dataset source
📁 Project Structure
📦 Netflix-Power-BI-Dashboard
 ┣ 📂 data
 ┃ ┗ 📄 netflix_clean.csv
 ┣ 📂 images
 ┃ ┗ 🖼️ dashboard.png
 ┣ 📂 dashboard
 ┃ ┗ 📄 NETFLIX_DASH.pbit
 ┗ 📄 README.md
🚀 How to Use
Clone the repository
bash
   git clone https://github.com/<your-username>/Netflix-Power-BI-Dashboard.git
Install Power BI Desktop (free, Windows).
Open dashboard/NETFLIX_DASH.pbit.
When prompted, point the data source to data/netflix_clean.csv.
Click Load and explore the dashboard! 🎉
🔮 Future Improvements
 Add a Top Directors / Actors page
 Add monthly seasonality analysis
 Add duration analysis (movie length, seasons per show)
 Publish to Power BI Service with a live link
 Add drill-through pages for individual titles
👤 Author

Your Name

LinkedIn GitHub Email

<div align="center">

⭐ If you like this project, give it a star! ⭐

Dataset credit: Kaggle. This project is for educational purposes and is not affiliated with Netflix.

</div>
