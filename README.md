# Power BI DAX Formulas – Productivity & Study 

## 📊 Overview
This project demonstrates the use of **Power BI DAX formulas** to analyze productivity, screen time, study hours, and user behavior metrics.  
The dashboard consolidates multiple KPIs into a single interactive view, providing actionable insights into user performance patterns.

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

*(Full list of measures is documented in the project files.)*

## 📈 Dashboard Preview
<img width="1168" height="658" alt="dax metrics" src="https://github.com/user-attachments/assets/7e48ed71-e974-4a15-b113-94c940b140e9" />



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
