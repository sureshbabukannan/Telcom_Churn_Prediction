# Telcom Churn dataset - Analysis and prediction

## Movtivation for the analysis
Telecom is very competitive industry. One of the key factor to be profitablity run the telcom bussiness in telecom industry is to retain customer. With the available data I have attempted to understand the factors contributing the customer churn and predict probability of customer who could move on. The results could help proactively intervention to prevent customer from moving out.

The Telco churn dataset contain details of customers who left the services of telcom company in past month along with other customers who stayed. The purpose of the is project is to answer questions on dataset 
> 1. What are many features contributing to the customer Churn ?
> 2. What is the probalility of a given customer who could churn ?

The dataset is available on [Kaggle](https://www.kaggle.com/blastchar/telco-customer-churn) and can be downloaded freely

> Features are of the datasets are 
>> * customerID 
>> * gender - Whether the customer is a male or a female
>> * SeniorCitizen - Whether the customer is a senior citizen or not (1, 0)
>> * Partner - Whether the customer has a partner or not (Yes, No)
>> * Dependents - Whether the customer has dependents or not (Yes, No)
>> * tenure - Number of months the customer has stayed with the company
>> * PhoneService - Whether the customer has a phone service or not (Yes, No)
>> * MultipleLines - Whether the customer has multiple lines or not (Yes, No, No phone service)
>> * InternetService - Customer’s internet service provider (DSL, Fiber optic, No)
>> * OnlineSecurity - Whether the customer has online security or not (Yes, No, No internet service)
>> * OnlineBackup - Whether the customer has online backup or not (Yes, No, No internet service)
>> * DeviceProtection - Whether the customer has device protection or not (Yes, No, No internet service)
>> * TechSupport - Whether the customer has tech support or not (Yes, No, No internet service)
>> * StreamingTV - Whether the customer has streaming TV or not (Yes, No, No internet service)
>> * StreamingMovies - Whether the customer has streaming movies or not (Yes, No, No internet service)
>> * Contract - The contract term of the customer (Month-to-month, One year, Two year)
>> * PaperlessBilling - Whether the customer has paperless billing or not (Yes, No)
>> * PaymentMethod - The customer’s payment method (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic))
>> * MonthlyCharges - The amount charged to the customer monthly
>> * TotalCharges - The total amount charged to the customer
>> * Churn - Whether the customer churned or not (Yes or No)

## Installation

The **Telco_customer_churn.ipynb** is the Jupyter notebook which contains data analysis and prediction models.
The data is from Telco-Customer-Churn.csv . This file should be in same folder as Telco_customer_churn.ipynb

As a prequisite Anaconda 3 or above package should be installed to execute the juypter Notebook. 

To start running the Telco_customer_churn.ipynb Juypter notbook 
> 1. Start the Anaconda promt
> 2. Navigate to directory where Telco_customer_churn.ipynb is stored
> 3. Type command Juypter Notebook to start Jupyter notebook environment. 
> 4. Open the Telco_customer_churn.ipynb in the Jupyter notebook file list displayed
> 5. On the menu bar click Cells > Run all 

## Usage

```
(base) Conda prompt> jupyter notebook Telco_customer_churn.ipynb
```

## Modeling 
The dataset is wrangled to cast the categorical columns to Character. Exploratory analysis is data to find the major features contributing to Churn. 
Then the function is used to nunmeric encoding of categorical feature and dummy variable replacement for catergorical features. 
THese dataset is used fit the logistic regression model and random forest predict the churn.

Then the metrics from each of the model is compared to see which is best fit model for probability prediction.  
It is found that Logistic regression with the categorical variables replaced with dummy vairables is the best fit by overall score.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
Copyright (c) 2020 Sureshbabu K

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Credits

* I have heavely referenced [Kaggle Telecom churn prediction by Pavanraj](https://www.kaggle.com/pavanraj159/telecom-customer-churn-prediction) to complete this data models

* I have also consulted Pandas, Seaborn, numpy documentation and Stackoverflow content online.

* The license text choosen from [choosealicense](https://choosealicense.com/licenses/mit/)

