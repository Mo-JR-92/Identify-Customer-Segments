# Identify-Customer-Segments:
**This project is part of Udacity Machine Learning Cross-Skilling Nanodegree Program Part (2) Unsupervised Learning**


- In this project, I applied unsupervised learning techniques to identify segments of the population that form the core customer base for a mail-order sales company in Germany. 
- These segments can then be used to direct marketing campaigns towards audiences that will have the highest expected rate of returns.
- The data used in this project has been provided by Bertelsmann Arvato Analytics, and represents a real-life data science task.


## Here are all the steps for this project:
### Step 0: Load the Data

There are four files associated with this project (not including this one):

- `Udacity_AZDIAS_Subset.csv`: Demographics data for the general population of Germany; 891211 persons (rows) x 85 features (columns).
- `Udacity_CUSTOMERS_Subset.csv`: Demographics data for customers of a mail-order company; 191652 persons (rows) x 85 features (columns).
- `Data_Dictionary.md`: Detailed information file about the features in the provided datasets.
- `AZDIAS_Feature_Summary.csv`: Summary of feature attributes for demographics data; 85 features (rows) x 4 columns

Each row of the demographics files represents a single person, but also includes information outside of individuals, including information about their household, building, and neighborhood. You will use this information to cluster the general population into groups with similar demographic properties. Then, you will see how the people in the customers dataset fit into those created clusters. The hope here is that certain clusters are over-represented in the customers data, as compared to the general population; those over-represented clusters will be assumed to be part of the core userbase. This information can then be used for further applications, such as targeting for a marketing campaign.

## Step 1: Preprocessing


## Step 2: Feature Transformation

## Step 3: Clustering

### Step 3.1: Apply Clustering to General Population

### Step 3.2: Apply All Steps to the Customer Data

### Step 3.3: Compare Customer Data to Demographics Data


## Results:
- The proportion of customers in cluster 8 (32% vs 7%) is much larger(overrepresented) than the general population proportion, which means that the people in cluster 8 are the target audiance for the company.
- the underrepresented clusters are cluster 2 (0.5% vs 6%), cluster 4 (1.3% vs 7%), cluster 5 (7.8% vs 0.7%), cluster 10 (6.5% vs 1%) all of these clusters fit to the 6% or more general vs 2% or less customers which means that the group of persons in these clusters is outside of the target demographics. ( I chose cluster 5 to countinue with this analysis)

#### Analysing Cluster 8 (target audience for the company):

**what kinds of people are typified by this cluster? here are 20 of the most notable traits**
- (1) Age: 46 or more, (2) Gender: male, (3) has high financial interest, (4) money-saver, (5) investor.
- (6) high home ownership, (7) return type: low- returner, (8) Religious: more likely to be, (9) Rationality: high, (10) low sexual interests, (10) dutiful.
- (11) tradional-minded, (12) high or very high houshold income, (13) more likely to be in the west, (14) more likely to be in good neighborhood, (15) high purchasing power in the region they live in.
- (16) low movement, (17) lives in upper middel class, (18) decade: 60s, (19) Wealth: prosperous households, (20) Life Stage: older families and mature couples.

#### Analysing Cluster 5 (outside of the target demographics):

**what kinds of people are typified by this cluster? here are 20 of the most notable traits**
- (1) Age: younger than 45, (2) Gender: male, (3) low financial interest, (4) not a money-saver, (5) low or average invesment.
- (6) average or low home ownership, (7) return type: more likely to be heavy returner, (8) Religious: less likely to be, (9) Rationality: average, (10) high sexual interests, (10) not dutiful. 
- (11) not tradional-minded, (12) low or average houshold income, (13) more likely to be in the west, (14) more likely to be in average or poor neighborhood, (15) average purchasing power in the region they live in. 
- (16) high movement, (17) lives in lower middel class, (18) decade: 80s or 90s, (19) Wealth: Less Affluent Households, (20) Life Stage: Young Couples With Children.

**It's important to note that I didn't include any missing data for this analysis, which means that a big chunk of the data have been left out, the result might have been different if I included them, or if the number of missing data was not as large to begin with.**
