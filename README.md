**<div align="center">CUSTOMER PROFILE FOR UNITED STATES CLYCING INDUSTRY USING K-MEANS AND RFM MODEL</div>**

## **Project overview**
***
> create customer profile for the U.S. bike industry

|Research method | Exploratory Data Analysis | Environment and tool|
|---|---|---|
|Descriptive analysis | Univariate Non-graphical|Excel
|Graph analysis | Univariate graphical |Jupyter notebook
|Segment Analysis | Multivariate Non-graphical | Python programming language
|CRISP-DM | Multivariate graphical

## Supported Models
| Customer Segment | Customer Lifetime Value | Prediction |
|---|---|---|
|RFM analysis|Corhort Analysis|Decision Tree
|K-Means Clustering| BG/NBD|Linear Regression
|Elbow method| Gamma-Gamma
|Silhouette analysis| 

## Libraries requirement
|||||
|---|---|---|---|
| Scikit Learn | Lifetimes | Plotly | Matplotlib | 
|Seaborn | Numpy | Pandas | Datetime |
| Math | Warnings | Squarify | Yellowbrick|
| Scipy |
# Dataset description
The AdventurWorks excel file was used to collect the data for this research which is a sample Dataedo documentation - AdventureWorks - Microsoft SQL Server sample database.
## Features 
| **Feature** | **Describe** | **Feature** | **Describe**  |
| ----------- | ----------- | ----------- | ----------- |
| *SalesOrderLineKey* | A key to access each individual transaction listed on a sales order | *Category* | This data only include Bikes category |
| *CustomerKey* | A key to access individual customer information | *Order Quantity* | Number of each order |
| *ProductKey* | A key to access individual product information | *Customer* | Name of customer |
| *OrderDateKey* | A key to access individual date order information | *City* | City located of customer |
| *Date* | Order date | *Product* | Bikes in the United States |
| *Sales Amount* | Total payment amount of each sales order line | *State-Province* | Detail located of customer |
| *Model* | Bikes segment | *Country-Region* | This data only include United States |
| *Subcategory* | Subordinate type of Bikes | ----------- | ----------- |

### Scopes
#### _Time scope_
The dataset contains all the transactions occurring between 7/2017 and 6/2021.
#### _Space scope_
This study focuses solely on the U.S. bike industry and the bike category
# Business understanding
PROBLEM : 
- Only have basic customer data but want to know customer behaviour to plan marketing strategy accordingly.
- Understanding which customers to focus on
prediction tasks: 
    - how much will they spend in the future (Regression)
    - what probability will they make another purchase in the future (Classification)

QUESTION : 
- How to understand customer behaviour to plan marketing strategy accordingly?
- Which customers have the highest spend probability in the next 90-days
- Which customers have recently purchased but are unlikely to buy
- Which customers were predicted to purchase but didn’t

MEASURE : 
- A well clustered customer basen on basic data that we have.
- Custumer Lifetime Value
- A predicted number cluster of new customers
# Analysis process
![Untitled Diagram drawio](https://user-images.githubusercontent.com/92135945/201092251-72e82515-42aa-47e9-98b4-a00c47264411.png)

# Experimental results
## Traditional RFM
![output](https://user-images.githubusercontent.com/92135945/203559627-519c93a6-a507-4cf4-a06e-c9b159554f96.png)
## RFM model using K-Means results
| Cluster| Recency | Frequency | Monetary | Value |
| ----------- | ----------- | ----------- | ----------- |----------- |
| 0   | Low |Low |Low |Low value customers |
| 1   | Low |High|High |High value customers |
| 2   | High |Low |Low |Mid value customers |
# Customer Lifetime Value
## Cohort Analysis
Retention by Monthly Cohorts
![output11](https://user-images.githubusercontent.com/92135945/203560024-d3430742-603b-4fbe-a401-a412c5bd3895.png)
Average Order quantity by Monthly Cohorts
![output1](https://user-images.githubusercontent.com/92135945/203560049-a5fa1f05-188a-4d5e-ae6b-74f402a06a42.png)
Average Spend by Monthly Cohorts
![output](https://user-images.githubusercontent.com/92135945/203559995-727f9749-f9ce-4d3c-ae7c-9fd6b58c2d8f.png)
## BG/NBD
Beta Geometric / Negative Binomial Distribution known as BG-NBD Model. Also sometimes it comes up as “Buy Till You Die”. It gives us the conditional expected number of transactions in the next period.
## Gamma-Gamma
We use this model for predicting how much average profit we can earn for each customer. It gives us the expected average profit for each customer after modelling the average profit for the mass
# Comparasion
| Model| Number of clusters | Finding optimal K method | Directional approach |
| ----------- | ----------- | ----------- | ----------- |
| Traditional RFM | 11 | RFM ranking | Quantile analysis |
| K-means Clustering | 3 | Elbow method and Silhouette Score | Centroid initialization method |

# Prediction

||Decision Tree|Linear Regression|
|---|---|---|
|Score on train data| 1.0 | 0.5285717305457521
|Score on test data| 0.9990645463049579| 0.5253361596462358
|MAE |0.0018709073900841909 | 0.47077768206041265
|RMSE| 0.06117037502066161 |0.5355690227775272

# Conclusion
To some extent, it proves that RFM and K Means really give us the performance such as: saving money and time, easy to adjust, different number of clusters from original RFM which is the important point and need to be made clear, discuss with the team to decide the true business plan for trades.

About the practical impact on the bike market, we will take more test models and apply our method to confirm precisely in the other project. We will retain all of our research in this project to apply in testing, clustering and observation of the other data sets. Clustering in diverse areas and new data sets which can not be “clean” will give us the experiences, true and practical performances. That result can be more convincing and costful in reality.

**<div align="center">-END-</div>**

---