# Challenge 5 Financial Planning

## Introduction
The purpose of this project is to use API's and simulations in order to make better financial decisions.  We will be using Alpaca API and Free Crypto API to pull data.  Then we will use Monte Carlo simulate what could happen to our retirement portfolio.

## Data
Utilizing API's we are able to get up to date pricing for our Portfolio, and then display it in a graph.

```
columns = ['Amount']
index = ['Crypto', 'Stock/Bond']
savings_df = pd.DataFrame(savings_data,
                         columns = columns,
                         index = index
                         )
savings_df.plot(kind='pie', title = 'Portfolio 08/26/22', y = 'Amount', figsize = (8,8))
```

![crypto_stock](/Images/crypto_stock.PNG)

## Analysis
We use Monte Carlo simulation to determine if a riskier but 10 year retirement portfolio will out perform a conservative 30 year portfolio.

![10_year_risky](/Images/10_yr.PNG)

![30_year_conservative](/Images/30_yr.PNG)

## Conclusion
The riskier 10 year portfolio does provide the potential for a significant gain in a much shorter time period, however the lower end shows that this 80/20 split might be too risky.  The 30 year more conservative portfolio is likely the best bet.