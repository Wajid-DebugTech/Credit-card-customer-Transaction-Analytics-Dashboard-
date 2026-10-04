# Credit Card Customer and Transaction Analytics Dashboard

Analysis of credit card usage, customer spending, payments, credit utilization and customer risk,
using Python for data preparation and Power BI for the dashboard.

## Files

| File | Description |
|---|---|
| `CreditCard_Analytics.ipynb` | Data profiling, cleaning, new columns and answers to the 14 business questions |
| `CreditCard_Clean_Data.xlsx` | Clean data tables used by Power BI |
| `CreditCard_Dashboard.pbix` | Power BI dashboard (5 pages, 15 charts) |
| `CreditCard_Report.pdf` | Report with business problem, cleaning summary, analysis and recommendations |
| `Raw_Data/` | Original data files |

## Data

Kaggle dataset: [computingvictor/transactions-fraud-datasets](https://www.kaggle.com/datasets/computingvictor/transactions-fraud-datasets)

`transactions_data.csv` is 1.2 GB, so it is stored compressed and split into parts
(`Raw_Data/transactions_data.csv.xz.part1`, `part2`, ...) because GitHub allows only 100 MB per file.

To get the CSV back, run this inside the `Raw_Data` folder, then unzip the `.xz` file with 7-Zip:

```
copy /b transactions_data.csv.xz.part1 + transactions_data.csv.xz.part2 transactions_data.csv.xz
```

On Mac or Linux: `cat transactions_data.csv.xz.part* > transactions_data.csv.xz` and then `xz -d transactions_data.csv.xz`.

## Author

Sumayya Jabeen
