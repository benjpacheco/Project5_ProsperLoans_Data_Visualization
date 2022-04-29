
<h1 align="center">Prosper Loans Data Visualization</h1>

## Table of Contents
- [Installation](#installation)
- [Project Overview](#po)
- [Source of Data](#sourcedata)
- [Dataset](#dataset)
- [Results](#results)
- [Key Insights for Presentation](#kip)
- [Why this project?](#p) 


## Installation <a name="installation"></a>

You need to be able to work in a Jupyter Notebook on your computer. The following packages (libraries) need to be installed. You can install these packages via conda, pip, or by creating an environment from my environment.yml file.

- Pandas
- Matplotlib
- Seaborn
- conda env create -f environment.yml
  
## Project Overview <a name="po"></a>

This project has two parts that demonstrate the importance and value of data visualization techniques in the data analysis process. In the first part, I will use Python visualization libraries to systematically explore a selected dataset, starting from plots of single variables and building up to plots of multiple variables. In the second part, I will produce a short presentation that illustrates interesting properties, trends, and relationships that I discovered in the selected dataset. The primary method of conveying my findings will be through transforming exploratory visualizations from the first part into polished, explanatory visualizations. 

#### Source of Data <a name="sourcedata"></a>

* [Loan Data from Prosper](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1554486256021000) with [Prosper Data Dictionary to Explain Dataset's Variables](https://www.google.com/url?q=https://docs.google.com/spreadsheet/ccc?key%3D0AllIqIyvWZdadDd5NTlqZ1pBMHlsUjdrOTZHaVBuSlE%26usp%3Dsharing&sa=D&ust=1554486256024000)

### Dataset <a name="dataset"></a>

This data set contains information on peer to peer loans facilitated by credit company Prosper. There are 113,937 loans with 81 variables. For the purpose of this investigation I've taken the following variables: Term, LoanStatus, BorrowerRate, ProsperRating (Alpha), ListingCategory (numeric), EmploymentStatus, DelinquenciesLast7Years, StatedMonthlyIncome, TotalProsperLoans, LoanOriginalAmount, LoanOriginationDate, Recommendations and Investors.

 
### Results <a name="results"></a>

In the exploration, I found that there was a moderate relationship between loan amounts and the rates (BorrowerRate/BorrwerAPR) with several different Credit Grades/Prosper Ratings given to Prosper customers. For customers that have no credit we see an upward slope with the loan amounts increasing and APR. Grades E and D seem to have a negative slope which aligns with bivariate findings, while anything higher than those two we can see the slope getting less steep  in a positive trend therefore higher grade assigned to the loan means the loan amount and rates will go up. This was an interesting finding because plotting loan amounts and the rates gives us a negative trend line. The relationship between loan amounts and interest/APR wasn't exactly linear but it showed an obvious negative correlation trend since in general the lower loan amount thats given by Prosper is tied to a higher % rate which makes total sense for a credit issuing company. I was disappointed with the correlation factors of my predictors variables in choosing, I could of selected better predictor variables to compare with loan amounts. I figured monthly income would be a good indicator of wether someone would recieve a higher amount loan. 

Other than the main variable loan amounts I verified the relationship between the % rates.
The rates had a 1:1 relationship which was not surprising, they were directly related to each other as most findings showed that if APR rose the interest would rise in relation to that APR. 

## Key Insights for Presentation <a name="kip"></a>

For the presentation, I will focus on the distributions of the main variable along with the percentage rates (BorrowerRate/BorrowerAPR). Afterwards, I will introduce the categorical variables compared to the main variables. 

   
### Why this project? <a name="p"></a>

Data visualization is an important skill that is used in many parts of the data analysis process. **Exploratory** data visualization generally occurs during and after the data wrangling process, and is the main method that you will use to understand the patterns and relationships present in your data. This understanding will help you approach any statistical analyses and will help you build conclusions and findings. This process might also illuminate additional data cleaning tasks to be performed. **Explanatory** data visualization techniques are used after generating your findings, and are used to help communicate your results to others. Understanding design considerations will make sure that your message is clear and effective. In addition to being a good producer of visualizations, going through this project will also help you be a good consumer of visualizations that are presented to you by others.

