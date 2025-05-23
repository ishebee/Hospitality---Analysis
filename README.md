
# 🏨 Hospitality Data Analysis Project

This project explores booking and room data for an imaginary hotel chain using five datasets. The objective is to perform end-to-end data analysis to understand booking patterns, room demand, and capacity issues across multiple hotel properties.

## 📁 Dataset Description

The project uses the following CSV files:

- **Dim_Date.csv**: Calendar details for 3 months including day names.
- **Dim_Hotels.csv**: Metadata of hotel properties (e.g., property ID, name).
- **Dim_rooms.csv**: Types of rooms available across properties.
- **fact_booking.csv**: Booking data with timestamps, room IDs, and guest counts.
Note: The dataset was aquired as process of learning from codebasics.io

## 🔍 Analysis Process

### 1. Data Import & Exploration
- Overview of each dataset
- Visualizations:
  - Bar charts on Booking Platform, Customer Ratings, and Room Categories
- Identification of:
  - Unique properties
  - Booking distribution across properties
  - Days with overbooking
  - Properties with highest room capacity

### 2. Data Cleaning
- Handled negative values in guest counts
- Ensured consistency in room types and booking dates

### 3. Insights Generated
- Booking patterns by room and platform
- Days with overbooked properties
- Which properties require more rooms
- High-performing booking platforms

  ## Project Structure
- **File Type/** : Jupyter Notebook


## 📊 Tools & Technologies Used

- Python (Pandas, Matplotlib, Seaborn)
- Jupyter Notebook
- Data Cleaning & EDA techniques

## 📌 Key Learnings

- Practical implementation of data wrangling and visualization
- Identifying real-world issues such as overbooking and invalid data entries
- Effective use of grouped analysis to derive business insights
