# Data Dictionary — `churn-bigml-80.csv`

Reference for the telecom customer churn dataset used to build the dashboard (80% training split of the classic BigML telecom churn dataset).

| Column | Type | Description |
|--------|------|-------------|
| `State` | Text | U.S. state code of the customer |
| `Account length` | Integer | Number of days the account has been active |
| `Area code` | Integer | Telephone area code |
| `International plan` | Text | Whether the customer has an international plan (`yes` / `no`) |
| `Voice mail plan` | Text | Whether the customer has a voice mail plan (`yes` / `no`) |
| `Number vmail messages` | Integer | Count of voice mail messages |
| `Total day minutes` | Decimal | Total call minutes during the day |
| `Total day calls` | Integer | Number of day calls |
| `Total day charge` | Decimal | Billed charge for day usage |
| `Total eve minutes` | Decimal | Total call minutes during the evening |
| `Total eve calls` | Integer | Number of evening calls |
| `Total eve charge` | Decimal | Billed charge for evening usage |
| `Total night minutes` | Decimal | Total call minutes at night |
| `Total night calls` | Integer | Number of night calls |
| `Total night charge` | Decimal | Billed charge for night usage |
| `Total intl minutes` | Decimal | Total international call minutes |
| `Total intl calls` | Integer | Number of international calls |
| `Total intl charge` | Decimal | Billed charge for international usage |
| `Customer service calls` | Integer | Number of calls to customer service |
| `Churn` | Boolean | Target variable — whether the customer churned (`True` / `False`) |

## Usage Notes

- `Churn` is the target field driving all KPI cards and breakdown visuals in the dashboard.
- Usage minutes and charges follow the pattern: *charge = minutes × rate* within each time band.
- A high `Customer service calls` count is a well-known churn indicator worth highlighting in reports.
