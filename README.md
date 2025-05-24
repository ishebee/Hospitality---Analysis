# AtliQ Grands Hospitality Data Analysis

This project is part of the Codebasics.io Data Analyst Bootcamp where I analyzed an imaginary hotel chain called **AtliQ Grands**, which operates in multiple Indian cities. The goal was to analyze booking data and derive business insights to help the company regain market share and optimize its operations.

---

## Datasets Used

The following CSV files were analyzed:

- `fact_bookings.csv`: Detailed individual booking-level data.
- `fact_aggregated_bookings.csv`: Monthly aggregated booking KPIs.
- `dim_date.csv`: Date dimension with weekday/weekend tags.
- `dim_hotels.csv`: Metadata about hotels including city and category.
- `dim_rooms.csv`: Room categories and classification metadata.

---

## Data Cleaning Steps

- Removed extra whitespace and standardized string formats.
- Converted `booking_date`, `check_in_date`, and `checkout_date` columns to `datetime` objects.
- Removed duplicate entries from `fact_bookings`.
- Checked for and handled nulls.
- Standardized capitalization and labels across columns like `room_category`, `booking_platform`, and `booking_status`.

---

## Data Transformation

- Merged datasets using keys such as `property_id`, `room_id`, and `date`.
- Enriched `fact_bookings` with room and hotel information for better context.
- Calculated additional columns like:
  - `Occupancy Rate = booked rooms / room capacity`
  - `Revenue Realized vs Revenue Generated`
- Aggregated data by month, platform, city, and room type for comparative analysis.
- Flagged bookings by weekday vs weekend using `dim_date`.

---

## Key Analytical Areas

### Room Category Analysis
Room categories included:
- **Elite**
- **Executive**
- **Premium**
- **Suite**

**Elite rooms** were the top choice with the highest revenue per room. However, **Executive rooms** were booked more often but had lower unit revenue.

---

### Booking Platform Insights

- Top platforms: `Makeyourtrip`, `Bookusnow`, `Stayzilla`, `Direct Booking`.
- `Makeyourtrip` led in volume, but `Direct Booking` yielded better per-booking revenue.
- Suggested stronger push for direct bookings via loyalty incentives.

---

### Ratings and Satisfaction

- Most ratings were **4 or 5**, indicating good guest satisfaction.
- Ratings were linked with higher revenue and lower cancellation rates.
- Properties with consistent low ratings were flagged for further attention.

---

### Booking Status Breakdown

- Types: `Confirmed`, `Cancelled`, `No-show`.
- Cancellations formed nearly **18%** of total bookings.
- Premium rooms had the highest cancellation rate.

---

## KPIs Calculated

- **Total Revenue**
- **Occupancy Rate**
- **Average Daily Rate (ADR)**
- **Revenue per Available Room (RevPAR)**
- **Cancellation Rate**
- **Guest Ratings Distribution**

---

## Key Findings

- **Mumbai** led with over 40% of the total revenue.
- **AtliQ Exotica** was the best performing hotel.
- **Elite rooms** generated the most revenue.
- **Makeyourtrip** dominated volume; **Direct Booking** was most profitable.
- **Weekend stays** showed higher occupancy, ideal for surge pricing.
- **Cancellation and no-show losses** were significant (~20%).

---

## Recommendations

- Implement dynamic pricing for weekends.
- Promote direct bookings via rewards.
- Prioritize marketing of Elite rooms.
- Improve low-rated properties based on guest feedback.
- Revisit cancellation policies for Premium rooms.

---

## Tools Used

- **Python**
- **Pandas**
- **Matplotlib / Seaborn** for data visualization
- **Jupyter Notebook**

---

## Repository Structure

┣ 📄 Hospitality.ipynb
┣ 📄 fact_bookings.csv
┣ 📄 fact_aggregated_bookings.csv
┣ 📄 dim_date.csv
┣ 📄 dim_hotels.csv
┣ 📄 dim_rooms.csv
┗ 📄 README.md

## Conclusion
- This project gave me hands-on experience in data cleaning, transformation, exploratory analysis, KPI calculation, and deriving actionable insights for a business scenario. The workflow reflects a complete data analytics pipeline that adds value to hospitality management.

  _____________________________________________________________________________________________________________________
