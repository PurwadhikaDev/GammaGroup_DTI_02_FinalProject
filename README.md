# Hotel Booking Prediction

Contributors:
- Kevin Rio Harristyando
- Sekar Saraswati Wibowo
- Theresia Diah Kusumaningrum

## Project Overview 

In the hospitality industry, web reservations are the trend, offering convenience to travelers and expanded reach to hotels. All the same, with this shift has come a significant wave of booking cancellations that is proving difficult to hotel operations and revenue management. Studies have reported 19% of cancellations coming from a hotel's website, 39% from Booking.com, and 25% from Expedia in the course of a four-month period. (sources)

Several factors contribute to this large number of cancellations:

- Guests prefer booking multiple hotels simultaneously, planning to finalize a decision closer to the date of arrival. This practice makes it more likely to have cancellations as travelers limit their options.(sources)

- Free cancellation as an option encourages guests to reserve rooms with no strings attached, making cancellations more likely.

- Unforeseen situations such as bad weather, strikes, computer failures, or personal emergencies might disrupt travel schedules, leading to last-minute cancellations.

### Problem Background & Stakeholders
The hotel industry faces significant challenges related to booking cancellations, which can impact revenue, operational efficiency, and overall customer satisfaction. Key stakeholders include:

- **Hotel Management:** Seeks to minimize revenue loss due to last-minute cancellations.
- **Revenue Management Teams:** Need accurate cancellation predictions to implement dynamic pricing and optimize room allocation.
- **Marketing Departments:** Can target customers more effectively by understanding cancellation patterns.
- **Business Strategy Teams:** Focus on evaluating campaign effectiveness, measuring ROI, and developing actionable strategies for growth.

## Analytical Approach

### Evaluating Model Performance: Understanding False Positives and False Negatives

When predicting hotel booking cancellations, it is crucial to understand the implications of false positives and false negatives, as they directly impact revenue management and operational planning.

#### False Positives (FP)
- **Definition:**  
  The model predicts that a booking will be canceled, but in reality, it is not canceled.
- **Business Impact:**  
  - Wasted retention efforts (discounts or promotions given unnecessarily)

#### False Negatives (FN)
- **Definition:**  
  The model predicts that a booking will not be canceled, but in reality, it is canceled.
- **Business Impact:**  
  - **Lost Revenue:** When a cancellation is not predicted, the hotel may prepare for the guest's arrival (e.g., staffing, inventory, and service preparations) and incur associated costs, only to have the room remain vacant.
  - **Missed Rebooking Opportunities:** A false negative can prevent the hotel from proactively rebooking the room, leading to significant revenue loss.
  
### Deciding Which is More Critical: FP or FN?
- **False Negatives are more critical.**  
  In the context of hotel booking cancellation prediction, failing to identify a cancellation (FN) can lead to unoccupied rooms and lost revenue opportunities.

### Choosing Evaluation Metrics for Booking Cancellation Prediction
  
- **F2 Score:**  
  To find balance between recall and precision, with more emphasize on recall, using the F2 Score is essential. This metric helps in managing the trade-off between catching as many cancellations as possible (recall) while avoiding too many false alarms (precision) that can lead to unnecessary overbooking strategies.

- **Recall:**  
  Recall is the most critical metric in this scenario. A high recall ensures that the model captures as many actual cancellations as possible, minimizing the risk of unanticipated vacant rooms.


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


### Reccommendation

## Tableau Dashboard


## Streamlit Application
