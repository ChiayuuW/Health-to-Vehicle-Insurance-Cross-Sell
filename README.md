# Health-to-Vehicle-Insurance-Cross-Sell

## About
This project predicts whether existing health insurance customers are likely to purchase vehicle insurance from the same company. The goal is to support cross-sell opportunities by identifying potential buyers.
- Business Impact: Helps optimize marketing strategies, reduce missed opportunities, and increase revenue.
- Focus: High recall, so the model minimizes the risk of missing potential customers.

## Dataset
## Data
| Variable                   | Type                       | Description                                                                                       |
| -------------------------- | -------------------------- | ------------------------------------------------------------------------------------------------- |
| **id**                     | Identifier                 | Unique ID assigned to each customer.                                                              |
| **Gender**                 | Categorical                | Gender of the customer (`Male`, `Female`).                                                        |
| **Age**                    | Numerical                  | Age of the customer in years.                                                                     |
| **Driving\_License**       | Binary                     | Whether the customer has a driving license (`1 = Yes`, `0 = No`).                                 |
| **Region\_Code**           | Categorical                | Encoded region code representing the customer’s residential area.                                 |
| **Previously\_Insured**    | Binary                     | Whether the customer already has vehicle insurance (`1 = Yes`, `0 = No`).                         |
| **Vehicle\_Age**           | Categorical                | Age of the customer’s vehicle (`< 1 Year`, `1–2 Year`, `> 2 Years`).                              |
| **Vehicle\_Damage**        | Binary                     | Whether the customer’s vehicle has been damaged in the past (`Yes = 1`, `No = 0`).                |
| **Annual\_Premium**        | Numerical                  | The yearly premium amount the customer pays for health insurance.                                 |
| **Policy\_Sales\_Channel** | Categorical (numeric code) | Encoded channel used to reach out to the customer (e.g., agents, phone, email, in-person).        |
| **Vintage**                | Numerical                  | Number of days the customer has been associated with the company.                                 |
| **Response**               | Binary (Target)            | Whether the customer is interested in vehicle insurance (`1 = Interested`, `0 = Not Interested`). |

## Exploratory Data Analysis (EDA)
- Visualized categorical vs. target (stacked bar charts with percentages)
- Density plots for numerical features vs. target
- Observed class imbalance (Response=0 ≫ Response=1)

## Key Insights
- Older customers and those with prior vehicle damage are more likely to purchase vehicle insurance.
- Customers already having vehicle insurance show extremely low interest (Previously_Insured=1).
- Cross-sell potential lies mainly in customers without prior vehicle insurance and with older/damaged vehicles.
