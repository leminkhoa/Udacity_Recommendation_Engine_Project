<h1>Recommendations with IBM</h1>

**Table of Contents**
- [Project Overview](#project-overview)
- [Model Tasks](#model-tasks)
- [File Description](#file-description)

# Project Overview
For this project we will analyze the interactions that users have with articles on the IBM Watson Studio platform, and make recommendations to them about new articles you think they will like. Below is an example of what the dashboard could look like displaying articles on the IBM Watson Platform.

Expect final results are as below:
![New in the community](IBM Watson Platform.png)

# Model Tasks
1. Exploratory Data Analysis:
   -  Explore input data
   -  Visualize our inputs and clean if needed
2. Rank Based Recommendations:
   - Find most popular articles based on most interactions (Used for new users that haven't had any reading history previously)
3. User-User Based Collaborative Filtering:
   - Look at users that are similar in terms of items they have interacted
   - Then recommend to chosen user based on neighbor users
4. Matrix Factorization:
   - Convert user-item matrix to 3 sub matrix: U, S, VT
   - Split data to train and test set
   - Predict and validate our model performance
   - Recommendations to improve if needed

# File Description
Our workspace is organized as below:
  - **data folder**: include data to used for our project
      - articles_community.csv # detailed information of each article
      - user-item-interactions.csv # user logs when they interacted with IBM articles
  - **Recommendations_with_IBM.ipynb**: Our main notebook to build recommendation models
  - **Recommendations_with_IBM.html**: Notebook's final version in html 
  - Remaining files are used for unit testing and storing our processed results