# TASK_10_DA


📊 Job Listings Scraping & Analysis – Task 10
🎯 Objective

To collect job listing data (title, company, location, salary, skills) and perform basic analysis to find:

Total jobs

Top locations

Most in-demand skills

Visualize job trends using a pie chart

🛠 Tools & Libraries

Python

pandas – data cleaning & analysis

matplotlib – visualization

re – text cleaning (regex)

collections.Counter – skill frequency count

📑 Data Source

Initially attempted live scraping from Indeed / TimesJobs / Naukri, but faced:

Blocking (anti-bot protection)

Dynamic content (JavaScript-rendered job cards not visible to BeautifulSoup)

Very few available jobs → empty results

✅ Solution: Used a public Kaggle dataset (glassdoor_jobs.csv) that contains hundreds of job postings, including job title, company, location, salary, and descriptions.

🔧 Steps Performed

Loaded dataset into pandas DataFrame

Renamed columns for consistency

Cleaned text fields (removed newline, tabs, bullets)

Counted jobs and displayed total

Analyzed locations – top 5 most frequent job locations

Extracted skills from job descriptions using regex + word frequency

Visualized top 5 locations using a pie chart

Saved cleaned dataset to CSV for reproducibility

📊 Results

Total Jobs Analyzed: 600+

Top Locations: New York, San Francisco, Los Angeles, Seattle, Boston (pie chart plotted)

Most In-Demand Skills: SQL, Python, Excel, Tableau, Machine Learning, Communication

📈 Visualization

Pie Chart – Top 5 Locations:

(Generated in the notebook)

🚧 Challenges Faced

Live scraping from Indeed/TimesJobs/Naukri returned empty results due to bot detection

Had to add time.sleep() between requests (still blocked)

Finally switched to a public dataset to ensure reproducible results



<img width="1281" height="797" alt="TASK_10" src="https://github.com/user-attachments/assets/b3503e44-3476-4db6-9716-f864cbac375c" />
