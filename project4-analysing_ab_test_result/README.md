# Analyze A/B Test Results

For this project, you will be working to understand the results of an A/B test run by an e-commerce website. The company has developed a new web page in order to try and increase the number of users who "convert," meaning the number of users who decide to pay for the company's product. Your goal is to work through this notebook to help the company understand if they should implement this new page, keep the old page, or perhaps run the experiment longer to make their decision.

## Understanding the data

- The number of rows in the dataset: `294,478`
- The number of unique users in the dataset: `290,584`
- The proportion of users converted: `12%`
- The number of times the **new_page** and **treatment** don't match: `3,893`
- Do any of the rows have missing values? `No`

## Messy data

- How should we handle the rows where **landing_page** and **group** columns don't match? `Remove these rows`

## Updated dataframe

- The number of unique ids in df2: `290,584`
- The **user_id** for the non-unique id in df2: `773,192`
- The **landing_page** for the non-unique id: `new_page`
- The **group** for the non-unique id: `treatment`
- The value of **converted** column for the non-unique id: `0`

## Probability

- Probability of converting regardless of page: `0.1196`
- Given that an individual was in the control group, the probability of converting: `0.1204`
- Given that an individual was in the treatment group, the probability of converting: `0.1188`
- The probability of receiving the new page: `0.5001`

## Hypothesis testing

- **p_new** under the null: `0.1196`
- **p_old** under the null: `0.1196`
- **n_new**: `145,310`
- **n_old**: `145,274`
- **p_new - p_old** under the null: `0`