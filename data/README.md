# Dataset

`uber_request_data.csv` contains the ride-request data used for the Power BI Supply & Demand Gap Analysis.

## Main Fields

The project documentation identifies the following fields:

- Request ID
- Pickup Point
- Status
- Driver ID
- Request Timestamp
- Drop Timestamp

## Data Interpretation

The dataset contains meaningful missing values.

- `Driver ID` can be missing when no cars are available.
- `Drop Timestamp` can be missing when a request is cancelled or when no car is available.

Therefore, these missing values should not automatically be interpreted as data-quality errors.

## Derived Analysis Fields

The project created additional fields for analysis:

- **Request Time**
- **Time Period**
- **Supply Gap**

The `Supply Gap` classification groups:

- completed/successful trips as **Supply**
- cancelled requests and requests with no cars available as **No-Supply**

## Dataset Size

The Power BI analysis contains **6,745 ride requests**.

## Source & Publication Note

The project report states that the dataset was obtained from Kaggle and imported into Power BI Desktop.

The exact Kaggle dataset URL and redistribution license are:

**Not confirmed from the uploaded files.**

For that reason, this repository should not imply ownership of the original dataset.
