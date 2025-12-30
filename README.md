# 📊 Global LinkedIn Data Science Profiles — Scraping, Analysis & Visualization

## 🧾 Overview

This project explores the career landscape of **Data Science professionals around the world** by extracting publicly available LinkedIn profile information and transforming it into meaningful insights.
It combines **manual dataset preparation**, **automated web scraping**, and **extensive data analysis** to reveal trends in:

* Career trajectories
* Skillsets and expertise
* Preferred tech stacks
* Educational backgrounds
* Job roles and industry pathways

The results aim to help students, professionals, and organizations make **strategic decisions about learning, hiring, and networking** within the Data Science domain.

---

## 🚀 Project Motivation

Data Science is a rapidly evolving field, yet many aspiring professionals lack visibility into:

* What skills are actually needed?
* How do successful Data Scientists build their careers?
* Which degrees or certifications matter most?
* What industries hire Data Scientists the most?

This project was created to answer those questions through **real-world data**, not assumptions.

---

## 🏗️ Project Workflow

### **1️⃣ Manual Data Collection (Phase 1)**

Before automation, a small dataset was collected manually to:

* Understand LinkedIn page structure
* Identify fields worth scraping
* Validate feasibility
* Create labels for testing our scraping logic

This foundational work helped refine the scraping plan so automated scripts could work reliably.

---

### **2️⃣ URL Scraper (Phase 2)**

Once pattern consistency was confirmed, a scraper was developed to:

* Search LinkedIn for Data Science-related roles
* Extract profile URLs
* Save them into a structured dataset

**Technologies:** Selenium, BeautifulSoup, Requests, Regex, Python

---

### **3️⃣ Data Field Scraper (Phase 3)**

A second scraper was then built to visit each collected URL and extract:

| Field                | Description                          |
| -------------------- | ------------------------------------ |
| Name                 | Full name of professional            |
| Current Job Title    | Current DS-related role              |
| Company              | Organization currently employed      |
| Previous Experiences | Job history + transitions            |
| Skills               | Technical & soft skills endorsed     |
| Education            | Degree, institution, graduation year |
| Certifications       | DS-related certifications            |
| Location             | Country/region (geographic insights) |

This step required handling:

* Lazy-loaded LinkedIn content
* Conditional data layouts
* Anti-scraping triggers
* Dynamic scrolling + CSS selectors

---

### **4️⃣ Data Cleaning, Processing & Storage (Phase 4)**

After scraping, data was cleaned and standardized:

* Duplicate removal
* Missing value handling
* Standardized country names
* Grouping job titles into DS categories
* Skill clustering

Data stored as:

* CSV files
* JSON references
* Pandas DataFrames for further analysis

---

### **5️⃣ Data Analysis & Visualization (Phase 5)**

Using Python analytics tools, we performed:

**Core Insights**

* Most common Data Science pathways
* Most in-demand skills (Python, SQL, ML, cloud, NLP, etc.)
* Popular companies hiring DS talent
* Degree vs. non-degree entry — who gets hired faster?
* Regional heatmaps showing global DS demand

**Tools**

* Pandas, NumPy
* Matplotlib, Seaborn, Plotly
* GeoPandas (for location heatmaps)

---

## 📈 Key Results (Examples of Findings)

*(You may adjust based on real results once analysis is finalized)*

* Data Scientists often transition from Software Engineering or Mathematics backgrounds.
* Python, SQL, Machine Learning, and Statistics are the most universally required skills.
* Certifications (Coursera, Google DS, IBM DS) are common among recent graduates.
* The U.S., India, U.K., and Germany hold the highest number of DS profiles in the dataset.

---

## 🧠 Future Enhancements

| Planned Feature               | Purpose                                        |
| ----------------------------- | ---------------------------------------------- |
| Machine Learning Models       | Predict future DS hiring trends                |
| NLP Analysis on Profile Text  | Auto-classify skills & extract insights        |
| Trend Visualization Dashboard | Deploy interactive web dashboard via Streamlit |
| Resume Recommendation Engine  | Suggest skills & projects for job seekers      |

---

## 📦 Tech Stack

**Languages & Tools**

* Python
* Selenium, BeautifulSoup, Requests
* Pandas, NumPy
* Matplotlib, Seaborn, Plotly
* Jupyter Notebook
* Git / GitHub

---

## 🛠️ How to Run Locally

```bash
# Clone repository
git clone https://github.com/yourusername/LinkedIn-DS-Scraper.git
cd LinkedIn-DS-Scraper

# Install dependencies
pip install -r requirements.txt

# Run URL scraper
python scripts/url_scraper.py

# Run profile scraper
python scripts/profile_scraper.py

# Run analysis notebook
jupyter notebook
```

⚠️ **Note** — Scraping LinkedIn violates Terms of Service if done without permission.
This project is for learning and research only. Use responsibly.

---

## 👨‍💻 Author

**Aneeq Ashraf**
BS Data Science — Air University, Islamabad
Passionate about Machine Learning, AI, and Data-Driven Projects

---

## ⭐ Support

If you found this project useful, consider giving the repository a **star ⭐** on GitHub — it helps showcase the work!
