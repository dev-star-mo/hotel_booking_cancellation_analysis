# Hotel Booking Cancellation Analysis

## Project Overview & Business Problem

Hotel bookings generate massive operational data, but booking volume alone doesn't guarantee future occupancy. High cancellation rates disrupt staffing, revenue forecasting, and room allocation.

This project analyzes hotel booking data to uncover patterns in **booking cancellations**. By understanding who cancels, where they come from, and what types of hotels they book, management can make smarter overbooking and operational decisions.

## Dataset & Preparation

The original dataset contained **119,390 bookings**. After cleaning (handling missing values in `agent`, `company`, and `children`, and removing duplicates), the final dataset contains

- *86,944 bookings**.

- *Key Engineered Features:**

- `total_nights`: Combined weekend and weekday stays.

- `total_guests`: Combined adults and children.

- `is_family`: Boolean flag for bookings with children/babies.

- `season`: Categorized arrival months into Winter, Spring, Summer, and Fall.

## Key Findings

1. **High Cancellation Risk:** The overall cancellation rate is **27.6%** (roughly 1 in 4

bookings).

2. **Hotel Type Matters:** City Hotels experience a significantly higher cancellation rate

(**30.04%**) compared to Resort Hotels (**23.70%**), likely due to business vs. holiday travel behaviors.

3. **Geographic Concentration:** A small number of top countries account for the vast

majority of both bookings and cancellations.

## Visualizations

### 1. Overall Cancellation Volume

![Overall Cancellation Status](https://github.com/dev-star-mo/hotel_booking_cancellation_analysis/blob/main/images/cancellation.png)

### 2. Cancellation by Hotel Type

![Cancellations by Hotel Type](https://github.com/dev-star-mo/hotel_booking_cancellation_analysis/blob/main/images/hoteltype.png)

### 3. Top 10 Countries

![Top 10 Countries](https://github.com/dev-star-mo/hotel_booking_cancellation_analysis/blob/main/images/countries.png)

## Strategic Recommendations

Based directly on the findings in the analysis, the following operational adjustments are recommended:

- **Implement an Overbooking Strategy:** Because the cancellation rate is 27.6% (meaning 1

in 3 bookings is cancelled), management must utilize an overbooking strategy to ensure the hotel is full on a given night.

- **Adjust Resource Planning:** The hotel cannot rely on the initial booking numbers for

staffing and food ordering.

- **Account for Hotel Type Volatility:** Operations should anticipate greater volatility in city

properties.

## 🛠 Tools & Skills Demonstrated

- **Languages & Libraries:** Python (Pandas, NumPy, Matplotlib, Seaborn)

- **Skills:** Data Cleaning (handling nulls/duplicates), Feature Engineering, Exploratory Data

Analysis (EDA), Data Visualization, and Business Analytics.

How to Run the Project

Clone the repository:

Bash

git clone [https://github.com/dev-star-mo/hotel_booking_cancellation_analysis.git](https://github.com/dev-star-mo/hotel_booking_cancellation_analysis.git)

cd hotel_booking_cancellation_analysis

Install dependencies:

Bash

pip install pandas numpy matplotlib seaborn jupyter

Open the notebook:

Bash

jupyter notebook hotel_booking_cancellation_analysis.ipynb
