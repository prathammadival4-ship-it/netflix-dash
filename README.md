<div align="center">
🎬 Netflix Content Analytics Dashboard

An interactive Power BI dashboard that explores the Netflix catalog by type, genre, country, rating, audience and year.

Show Image Show Image Show Image Show Image

Netflix Dashboard

</div>
📖 About

This project turns the Netflix Movies and TV Shows dataset from Kaggle into a dark, Netflix-style dashboard. The data was cleaned and enriched with Python (Pandas), then modeled in Power BI using Power Query and DAX. It has slicers for Type, Release Year, Audience and Director, KPI cards for total titles, movies and TV shows, plus charts for the Movies vs TV Shows split, titles by year, top 8 genres, top 8 countries and titles by rating.

📊 Dataset

netflix_clean.csv contains 5,336 titles and 20 columns, covering content released from 1942 to 2021. Besides the original Kaggle fields, I added year_added, month_added, primary_country, primary_genre, duration_value, duration_unit, content_age and audience (Kids / Teens / Adults).

💡 Key Insights
Insight	Result
Content split	~97% Movies, ~3% TV Shows
Top genres	Dramas (1,519), Comedies (1,127), Action & Adventure (806)
Top countries	United States (2,133), India (910), United Kingdom (347)
Main audience	Adults (2,602) and Teens (2,390)
Peak year for new titles	2019 (1,265 titles added)
🚀 How to Run

Clone the repo, open dashboard/NETFLIX_DASH.pbit in Power BI Desktop, point the data source to data/netflix_clean.csv when asked, and click Load.

📦 Netflix-Power-BI-Dashboard
 ┣ 📂 data        → netflix_clean.csv
 ┣ 📂 dashboard   → NETFLIX_DASH.pbit
 ┣ 📂 images      → dashboard.png
 ┗ 📄 README.md
👤 Author

Your Name · LinkedIn · GitHub · Email

<div align="center">⭐ If you like this project, give it a star! ⭐</div>
