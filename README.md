# ml-predictor

## Overview 
The idea behind “Real Estate Price Predictor” project was to apply Machine Learning techniques to predict real estate prices in a particular geography.

The key hypothesis that we wanted to test is that leveraging variables like geographic location, house size, historic house prices and median income in a particular location could serve as good predictors for future house prices.

We also wanted to understand what, if any, limitations exist when using the above inputs to predict future house prices


## Data Summary  

Two input data files were used to build the model:
Historical house sales data for NY state for the past 20+ years that contained zip codes, house sizes, # of beds and baths, dates of house purchases, house prices

Medium household incomes by zip codes in NY state
Historical house prices were adjusted to inflation using 3% yearly inflation rate

Random Forrest and Linear Regression were initially used to predict future house prices in NY state

After evaluating initial results, we decided to leverage Random Forrest model that was delivering more accurate predictions compared to Linear Regression



### Linear Regression Model: Show the Importance of Adjusting for Inflation
- Option 1: NOT Adj-ed price by inflation < $10MM; All features 
    - [Colab Notebook](https://drive.google.com/file/d/1WQcjcwG7j3dCn1n6rJHKZh-j1DYZJ7zL/view?usp=sharing)

- Option 2 - Adj-ed price by inflation < $10MM; All features 
    - [Colab Notebook](https://drive.google.com/file/d/17bpFn2w5ZPTfsFggHYK-2BRtuFylCtCW/view?usp=sharing)




### Random Forrest models:
- Option 1: No Income, Adj-ed price. R^2: = 0.918
    - [Colab Notebook](https://drive.google.com/file/d/1lm6FSZkOjQHrh370gFHIOv4Cb1ttPVtX/view?usp=sharing)

- Option 2: Income, Adj-ed price. R^2: = 0.976
    - [Colab Notebook](https://drive.google.com/file/d/1VW0u7EV1SOhQ3hfOtzSRNjJALdIyeVSz/view?usp=sharing)

- Option 3 - Income, Adj-ed price < $2MM 0.959 
    - [Colab Notebook](https://drive.google.com/file/d/1ntigbYutpz98qIb6KCoG0gpw17y-YJcn/view?usp=sharing)




