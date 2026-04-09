# Hotel Booking Data Science Project

## Project Overview
This project analyzes hotel booking data to understand cancellation patterns and guest behavior. The main focus is on **data cleaning, feature engineering, exploratory data analysis (EDA), and preparing data for machine learning**.

Key goals:
- Identify factors affecting cancellations  
- Engineer meaningful features like `total_guests` and `is_family`  
- Encode categorical variables for ML  
- Visualize trends and correlations  

---

## Dataset Features

### Numeric Features
- `lead_time` – Days between booking and arrival  
- `stays_in_weekend_nights` – Weekend nights booked  
- `stays_in_week_nights` – Week nights booked  
- `total_guests` – Sum of adults, children, and babies  
- `num_kids` – Children + babies  
- `adr` – Average daily rate  
- `days_in_waiting_list`  
- `booking_changes`  
- `total_of_special_requests`  

### Categorical Features (encoded)
- `hotel` – City Hotel / Resort Hotel (one-hot encoded)  
- `meal`, `market_segment`, `distribution_channel`, `deposit_type`, `customer_type`, `reserved_room_type` (one-hot encoded)  
- `arrival_date_month_combined` – Month of arrival in calendar order  
- `is_repeated_guest`, `is_family` – Binary flags  

### Target Variable
- `is_canceled` – 0 = Not canceled, 1 = Canceled  

---

## Data Science Workflow

1. **Data Cleaning**
   - Remove unnecessary columns like `agent`, `company`, `reservation_status`  
   - Handle missing values  

2. **Feature Engineering**
   - Combine guests → `total_guests`  
   - Create `num_kids` and `is_family` flags  
   - Encode categorical variables for ML  
   - Combine month dummies into `arrival_date_month_combined`  

3. **Exploratory Data Analysis (EDA)**
   - Bar plots, line plots, boxplots, histograms  
   - Correlation heatmaps of numeric features  
   - Multi-category analysis (e.g., hotel × deposit_type)  

4. **ML Preparation**
   - Only numeric and encoded features remain  
   - Target variable: `is_canceled` ready for ML models  

---

## Usage

1. Load the cleaned dataset into Jupyter Web or Python environment  
2. Explore the dataset using visualizations or summary statistics  
3. Prepare features and target for ML experiments  

---

## Dependencies

- Python 3.x  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## Author

**Yahia** – Data Scientist & Python Enthusiast  
Focus on hotel booking analytics, EDA, and cancellation prediction.