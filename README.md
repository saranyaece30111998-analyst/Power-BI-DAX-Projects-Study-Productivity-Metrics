# 📊 Productivity & Study Dashboard Report 

## 1. Executive Summary
This project leverages **Power BI DAX formulas** to analyze user productivity, screen time, study hours, and behavioral patterns.  
The dashboard provides actionable insights into how study habits, free time, and sleep quality influence overall productivity.

---

## 2. Objectives
- Build a **DAX-driven dashboard** for productivity analysis.  
- Identify **high vs. low productivity users**.  
- Highlight the impact of **screen time and sleep quality**.  
- Rank users by **study hours and free time**.  
- Demonstrate **business-ready KPIs** for portfolio and interview use.

---

## 3. Key Metrics & KPIs
- **Average Productivity:** 37.61  
- **Total Productivity:** 225.68K  
- **Total Screen Time:** 41.52K  
- **Average Free Time:** 6.50 hours  
- **Average Active Time:** 10.99 hours  
- **High Productivity Users:** 1,376  
- **Low Productivity Users:** 3,445  
- **Top 5 Study Hours:** 87.91 hours  
- **Good Sleep Users:** 1,259  

---

## 4. Dashboard Highlight
<img width="1168" height="658" alt="dax metrics" src="https://github.com/user-attachments/assets/8a422c96-b2c6-425a-87c2-5745ff8df8aa" />


- **KPI Panels:** Productivity, screen time, study hours, free time.  
- **Segmentation:** High vs. low productivity, sleep quality impact.  
- **Tables:**  
  - Ranked study hours (Top 5 users).  
  - Screen time distribution.  
  - Free time leaders.  

---

## 5. DAX Formulas
Examples of DAX measures used:
- `Average Productivity = AVERAGE(Productivity[Value])`
- `Total Productivity = SUM(Productivity[Value])`
- `Average Free Time = AVERAGE(Users[FreeTime])`
- `Top Study Hours = TOPN(5, Users, Users[StudyHours], DESC)`
- `Screen Time Rank = RANKX(ALL(Users), SUM(Users[ScreenTime]))`

*(Full list of measures is included in the project files.)*

---

## 6. Key Insights
- 📉 **High screen time** correlates with lower productivity.  
- 💤 **Good sleep** improves average productivity (42.00).  
- 📈 **Top study hour users** consistently outperform peers.  
- ⏱️ **Low productivity users** tend to have more free time (7.38 hrs).  

---

## 7. Dataset Overview
- **User



## 🛠️ Key Features
- **Average & Total Productivity** tracking
- **Screen Time Analysis** (high vs. low usage)
- **Study Hours Ranking** with top 5 users
- **Free Time & Active Time Metrics**
- **Sleep Quality Impact** on productivity
- **Addiction vs. Productivity Trends**

## 🔑 DAX Measures Used
Some of the core DAX formulas applied:
- `Average Productivity = AVERAGE(Productivity[Value])`
- `Total Productivity = SUM(Productivity[Value])`
- `Average Free Time = AVERAGE(Users[FreeTime])`
- `Top Study Hours = TOPN(5, Users, Users[StudyHours], DESC)`
- `Screen Time Rank = RANKX(ALL(Users), SUM(Users[ScreenTime]))`


The dashboard panels include:
- **KPIs**: Average productivity, total screen time, study hours, free time
- **User Segmentation**: High vs. low productivity users
- **Tables**: Ranked study hours, screen time, and free time
- **Insights**: Sleep quality correlation with productivity

## 📂 Dataset
The dataset contains fields such as:
- `User ID`
- `Study Hours`
- `Screen Time`
- `Free Time`
- `Active Time`
- `Sleep Quality`
- `Productivity Metrics`

## 🚀 How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/dax-productivity-dashboard.git
