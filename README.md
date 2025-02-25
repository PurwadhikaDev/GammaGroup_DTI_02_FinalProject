# Hotel Booking Prediction

Contributors:
- Kevin Rio Harristyando
- Sekar Saraswati Wibowo
- Theresia Diah Kusumaningrum

## Project Overview 
The hotel industry faces significant challenges related to booking cancellations, which can impact revenue, operational efficiency, and overall customer satisfaction. Key stakeholders include:

- **Hotel Management:** Seeks to minimize revenue loss due to last-minute cancellations.
- **Revenue Management Teams:** Need accurate cancellation predictions to implement dynamic pricing and optimize room allocation.
- **Marketing Departments:** Can target customers more effectively by understanding cancellation patterns.
- **Business Strategy Teams:** Focus on evaluating campaign effectiveness, measuring ROI, and developing actionable strategies for growth.

### Data Understanding
- **Source:** [Hotel Booking Demand Dataset on Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand/data)
- **Description:**  
  This dataset contains 119,389 historical booking records from hotels, which include various features such as booking details, customer demographics, and booking statuses. Each row in the dataset represents a single booking record.

- **Target Variable:**  
  For our classification task, the target variable is **`is_canceled`**, where:
  - `1` indicates that the booking was canceled.
  - `0` indicates that the booking was not canceled.

### Modelling

We compared the results of 6 different classification algorithms and applied 2 undersampling methods to find the best model.
**Models**
- Logistic Regression
- KNN (K-Nearest Neighbors)
- Decision Tree
- Random Forest
- LightGBM (Light Gradient Boosting Machine)
- XGBoost (Extreme Gradient Boosting)

**Undersampling Methods**
- Random Undersampling
- SMOTE

### Result

## Tableau Dashboard


## Streamlit Application
