**<div align="center">CUSTOMER PROFILE FOR UNITED STATES CLYCING INDUSTRY USING K-MEANS AND RFM MODEL</div>**

## **Project overview**
***
> create customer profile for the U.S. bike industry
## Research method 
* Descriptive analysis
* Graph analysis
* Segment Analysis
* RFM model
* K-Means clustering
* Elbow method
* Silhouette analysis
* Customer Lifetime Value
## Environment and tool
* Excel
* Jupyter notebook
* Python programming language
#### Libraries
* Numpy
* Pandas
* Seaborn
* Scipy
* Matplotlib
* Scikit-learn
* Plotly
* Yellowbrick
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
PROBLEM : Only have basic customer data but want to know customer behaviour to plan marketing strategy accordingly.

QUESTION : How to understand customer behaviour to plan marketing strategy accordingly?

MEASURE : A well clustered customer basen on basic data that we have.
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
## Customer Lifetime Value
Retention by Monthly Cohorts
![output11](https://user-images.githubusercontent.com/92135945/203560024-d3430742-603b-4fbe-a401-a412c5bd3895.png)
Average Order quantity by Monthly Cohorts
![output1](https://user-images.githubusercontent.com/92135945/203560049-a5fa1f05-188a-4d5e-ae6b-74f402a06a42.png)
Average Spend by Monthly Cohorts
![output](https://user-images.githubusercontent.com/92135945/203559995-727f9749-f9ce-4d3c-ae7c-9fd6b58c2d8f.png)

# Comparasion
| Model| Number of clusters | Finding optimal K method | Directional approach |
| ----------- | ----------- | ----------- | ----------- |
| Traditional RFM | 11 | RFM ranking | Quantile analysis |
| K-means Clustering | 3 | Elbow method and Silhouette Score | Centroid initialization method |

# Conclusion
To some extent, it proves that RFM and K Means really give us the performance such as: saving money and time, easy to adjust, different number of clusters from original RFM which is the important point and need to be made clear, discuss with the team to decide the true business plan for trades.

About the practical impact on the bike market, we will take more test models and apply our method to confirm precisely in the other project. We will retain all of our research in this project to apply in testing, clustering and observation of the other data sets. Clustering in diverse areas and new data sets which can not be “clean” will give us the experiences, true and practical performances. That result can be more convincing and costful in reality.

**<div align="center">-END-</div>**
