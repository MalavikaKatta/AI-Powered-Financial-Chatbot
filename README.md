# AI-Powered Financial Chatbot

## Dataset

The dataset was created using 10-K documents from Microsoft, Apple, and Tesla. It includes financial data for three fiscal years, covering the following metrics:

<img src="https://www.thestreet.com/.image/ar_16:9%2Cc_fill%2Ccs_srgb%2Cfl_progressive%2Cq_auto:good%2Cw_1200/MTg2ODU3NDU5MjEyNjI1ODA4/big-tech-tesla-microsft-apple.jpg" width="500" height="300">

- **Total Revenue**
- **Net Income**
- **Total Assets**
- **Total Liabilities**
- **Cash Flow from Operating Activities**

![image](https://github.com/user-attachments/assets/edd967f6-0546-43dc-9e34-d8dfa8eb9b8c)

## How the Chatbot Works

The chatbot is designed to answer financial queries based on the dataset.

### Mechanism of the Chatbot:

1. **Keyword Identification**: The chatbot checks if the query contains specific keywords related to financial metrics.
2. **Data Matching**: It identifies and matches the keywords with the relevant columns in the dataset.
3. **Entity Recognition**: The chatbot recognizes company names and fiscal years mentioned in the query.

### Query Execution:

- If the query involves a financial metric without a specified company, the chatbot sums the values across all companies.
- If a specific company is mentioned, it retrieves the corresponding financial metric for the latest year or the specified year.
- If the query asks for a comparison, it calculates the difference between the values from the last two years.
- If the query seeks highest or lowest values, it determines the company with the maximum or minimum value for that metric in the given or latest available year.

## Predefined Queries Supported

1. **Total Values for Financial Metrics**:
   - What is the total net income?
   - Total revenue in 2024?

2. **Company-Specific Financial Data**:
   - What is the total net income for Microsoft in 2024?
   - What is the total revenue for Apple in 2023?

3. **Comparative Financial Analysis**:
   - How has net income changed over the last year?
   - How has revenue for Tesla changed over the last year?

4. **Finding the Highest and Lowest Values**:
   - Which company has the highest total revenue?
   - Which company has the lowest net income?

## Limitations

- The chatbot can only answer one question at a time and does not support follow-up queries.
- It provides answers in a predefined structured format and may not align perfectly with user question phrasing.
- If there is a spelling mistake in the company name, the chatbot may fail to return an answer.

![image](https://github.com/user-attachments/assets/490ceabe-321c-44d8-90cb-414972e42b6f)
