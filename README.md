# Amazon Purchase Spending Analysis

Exploring recorded Amazon spending across time, product categories,
respondent characteristics, and shipping destinations.

**Author:** Nilakshi Kakati  
**Tools:** Python with Pandas, Seaborn, and Matplotlib

## View the analysis

- [Jupyter notebook](Amazon_Purchase_Spending_Analysis.ipynb)
- [Download HTML report](Amazon_Purchase_Spending_Analysis.html)

To read the HTML report, download the file and open it in a browser.

## Project overview

This analysis examines 1,810,793 purchase records linked to
5,026 respondents during 2018–2022.

It explores annual and monthly spending, leading product categories,
median spending by respondent age and household income, and
shipping destinations.

## Key findings

- Recorded spending peaked in 2021 at USD 11.12 million.
  Average spending per respondent active that year was USD 2,287.14.
- The rise through 2021 and decline in 2022 remained when comparing
  the same 3,962 respondents with recorded purchases in all five years.
- Within that consistent group, pet food, gift cards, and chairs
  had the largest identified-category dollar increases from 2019 to 2020.
- December led monthly spending within each year from 2018 to 2021;
  July led in 2022.
- ABIS_BOOK led identified categories across 2018–2022 with
  USD 1.34 million in recorded spending.
- Respondents aged 45–54 had the highest median recorded spending.
  Median spending also increased across reported household-income ranges.
- California, Texas, and Florida led recorded spending among
  known shipping destinations.

## Approach

- Checked missing values, repeated rows, dates, and unusual prices
  and quantities.
- Calculated recorded spending as unit price multiplied by quantity.
- Selected 2018–2022 for the main comparisons.
- Validated survey respondent IDs before joining survey information.
- Compared annual averages using both changing yearly respondent
  groups and a consistent five-year group.
- Created seven visualizations with findings and limitations.

## Data source

[Open e-commerce 1.0 — Harvard Dataverse](https://doi.org/10.7910/DVN/YGLYDY)

[Accompanying research paper — Scientific Data](https://www.nature.com/articles/s41597-024-03329-6)

Files used:

- amazon-purchases.csv
- survey.csv
- fields.csv — survey question definitions

The source CSV files are not included in this repository.

## Run the notebook

1. Download the three CSV files from the dataset source.
2. Place them in your Downloads folder, or update the file paths
   in the notebook.
3. Install the required libraries:

   pip install pandas seaborn matplotlib jupyter

4. Open the notebook in Jupyter and run its cells from top to bottom.

## Limitations

Results describe this participant sample, not Amazon’s overall sales
or all U.S. shoppers. Available purchase histories vary, including
within the consistent respondent group.

Amazon accounts may be shared. Purchases linked to a respondent
may include purchases by other account users.

Household income covers the 12 months before the survey; spending
covers 2018–2022. Age and income comparisons are descriptive
and do not establish cause and effect.

Unknown categories account for 5.37% of recorded spending.
Shipping rankings exclude records with missing destinations.
Shipping states do not necessarily indicate respondents’ residences.

Repeated rows were retained because no order ID was available
to distinguish duplicates from separate purchases. Spending is
not verified net of refunds, tax, or shipping.
