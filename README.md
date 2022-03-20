# Group 3 Final Project
<div id="top"></div>
<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/ByronKrauskopf/Group_3_Final_Project/Resources/logo.png">
    <img src="https://github.com/ByronKrauskopf/Group_3_Final_Project/blob/main/Resources/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Best-README-Template</h3>

  <p align="center">
    Movie Recommendation ML Model
    <br />
    <a href="https://github.com/ByronKrauskopf/Group_3_Final_Project"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="#">View Demo</a>
    ·
    <a href="https://github.com/ByronKrauskopf/Group_3_Final_Project/issues">Report Bug</a>
    ·
    <a href="https://github.com/ByronKrauskopf/Group_3_Final_Project/issues">Request Feature</a>
  </p>
</div>

<!--################TABLE OF CONTENTS################-->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#project-overview">Project Overview</a>
      <ul>
        <li><a href="#project-inspirations">Project Inspirations</a></li>
        <li><a href="#data-source">Data Source</a></li>
        <li><a href="#targeted-shareholders">Targeted Shareholders</a></li>
        <li><a href="#questions-to-be-answered">Questions to be answered</a></li>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#relational-database-setup">Relational Database Setup</a></li>
        <li><a href="#erd-database-diagram">ERD Database Diagram</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#machine-learning-models">Machine Learning Models</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#communications-protocol">Communications Protocol</a></li>
    <li><a href="#contributing">Contributing</a></li>
  </ol>
</details>

<!--################About################-->
# Project Overview
__Movie Recommendation system from MovieLens dataset__

Welcome to our final data analytics project. This project aims to tell a cohesive story using a dataset. As a small team, we will create an impressive data visualization app, that will be a cumulative display of the skills we acquired throughout the bootcamp. 
Our chosen project will be to build a movie recommendation system. With many streaming services available nowadays, building an efficient movie recommendation system has become more important due to the increase in demand to create customized content for consumers. We will be using the MovieLens dataset to build a movie recommender system. It contains approximately 1,000,209 movie ratings of 3,900 movies made by 6,040 MovieLens users.  The reason we chose this topic is because we have a large dataset to work with and we all enjoy watching movies and are looking for a recommendation on what to watch next. The main questions we want to answer with the dataset is: 

## Project Inspirations
With many streaming services available nowadays, building an efficient movie recommender system has become more important due to the increase in demand to create customized content for consumers. We will be using the MovieLens dataset to build a movie recommender system. It contains approximately __movie ratings__ of movies made by __MovieLens users__. 

## Data Source
MovieLens 25M Dataset: https://grouplens.org/datasets/movielens/25m/

## Targeted Shareholders
The potential customers of our project are mainly movie corporations, directors, and producers. We hope our target customers could use our analysis to refer to the genres that are easiest to score in marketing and take it as a reference to their future filmmaking accordingly.

## Questions to be answered
The main question we want to answer with the dataset is: __Can we accurately predict movie suggestions for users based off their previous ratings?__
 - What genres of movies score high ratings in current market?
 - What genres of movies are likely to win awards?
 - What genres of movies are likely to have a high box office?

### Built With:
- AWS
- Postgres SQL + PgAdmin
- Python 3.4
- Tableau
- HTML
- JS
- Flask
<p align="right">(<a href="#top">back to top</a>)</p>

<!--#############Getting Started################-->
# Getting Started

### Prerequisites
- installation packages and software versions

### Relational Database Setup
Using a database connected with AWS is a convenient way to store different datasets that have relationships with each other.

Additional instructions to set up a PostgreSQL database instance with Amazon Web Services (AWS) can be found in this [link](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_GettingStarted.CreatingConnecting.PostgreSQL.html).

*Initial AWS DB setup instructions:*
1. Create and sign into your AWS Management console and open the Amazon RDS Console at https://console.aws.amazon.com/rds/.
2. In the upper-right corner of the AWS Managment Console, Choose the AWS Region where you will create the DB Instance. 
3. In the Navigation pane, choose **Databases**.
5. Choose **Create Databases.** and select the **Easy create** option.
6. On the **Create database** page, shown following, make sure that the **Standard create** option is chosen, and then choose **PostgreSQL**.
7. Under **Version**, click on the dropdown menu and select PostgreSQL 12.8-R1. This allows us to select the free tier for DB template.
9. For **Templates**, select **Free tier**.
10. Enter a name for the **DB instance identifier**.
11. For **Master username**, enter a name for the master user or leave it to the default name,
12. For **Master password**, enter a password or use an auto generated password by clicking the checkbox, **Auto generate a password**
13. Under the **Connectivity** section, click the **Additional connectivity configuration** drop down to display more options. Under **Publicly accessible** options, select **Yes**.
14. Scroll to the bottom and select **Create database** button. On the main AWS RDS dashboard, you should see your newly created database. It will take some time to be initialized and created. 

*Connecting the DB with pgAdmin:*
1. Navigate to the **Services** drop down tab and select **RDS**.
2. Under the **Resources** section, select **DB Instances** link.
3. Click the DB instance.
4. Copy the **Endpoint** under the **Connectivity & Security** section. This endpoint will be used to connect your pgAdmin to the AWS server. 
5. Navigate to pgAdmin and login.
6. Select **Add New Server** link. On the generated popup, enter a **Name** for the server name.
7. Click on the **Connection** tab and in the **Host name/address** box, paste in the copied endpoint.  
8. **Port** number should be defaulted at 5432, postgres should be the defaulted **Maintenance database** unless you choose a different username during the creation of the AWS DB.  
9. Fill out the **Password** that you used to create the AWS database. 
10. Click the blue **Save** button. You should have now successfully connected your AWS server to your pgAdmin. 

### ERD Database Diagram

![ERD](./Resources/ERD_image.png)

The schema can be viewed [here](https://github.com/ByronKrauskopf/Group_3_Final_Project/blob/main/Resources/ERD_schema.txt)

<p align="right">(<a href="#top">back to top</a>)</p>

<!--################Usage################-->

# Usage
- describe use case of our project

<p align="right">(<a href="#top">back to top</a>)</p>

<!--################Machine Learning Models #################-->

# Machine Learning Models

### **1 - Model Based Collaborative Filtering Using Matrix Factorization (MF)**

**The Model:** The model is a collaborative filtering method that finds the relationship between items and users’ entities. The model learns the latent preferences of users and the latent attributes of items from known ratings to find similarity and make a recommendation. The model uses low-rank matrix factorization to derive the preferences from the dataset. 

**Why we are using it:** The model can discover hidden correlation/features in the dataset, remove redundant and noisy features, and can access easier data storage and processing. 

**The Math:** The matrix factorization method used for this method is the ***Singular value decomposition (SVD)***. The algorithm takes a matrix in 

**Features of the model:** Movie ratings

**Predicted Output:** List of recommended movies

### **2 - Random Forest Classifiers**

**The Model:** Random forest classifiers are a kind of gathering learning model that joins various more modest models into a more vigorous and precise model. Random forest models utilize weak learner algorithms (choice trees) and join their result to make a last order (or regression) choice.

**Why we are using it:** Both result and component determination of irregular woodland models are not difficult to decipher, and they can undoubtedly deal with exceptions and nonlinear information. The random forest model can accomplish equivalent prescient exactness on large tabular data with less code and faster performance. Moreover, the Random Forest has a great interpretability and high accuracy

<div align="center">
  <img src="https://github.com/ByronKrauskopf/Group_3_Final_Project/blob/main/Resources/matrix.PNG" alt="rfc">
</div>
  
**The Math:** The model does a row and column sample with a decision tree as its base. By increasing the number of base learners (k), the variance of the model will decrease and the opposite happens if the number of base learners (k) increases. A *Gini* index is calculated to determine the impurity of nodes in the decision tree; typically a decision tree classifier will choose the node with the largest Gini index as the root node. 

<div align="center">
  <img src="https://github.com/ByronKrauskopf/Group_3_Final_Project/blob/main/Resources/decision_tree_model.PNG" alt="tree_model">
</div>

**Predicted Output:** The bootstrapping Random Forest calculation consolidates gathering learning techniques with the choice tree system to make various arbitrarily drawn choice trees from the information, averaging the outcomes to yield another outcome that regularly prompts solid predictions/classification.

### **3 - Memory-Based Item-item Collaborative Filtering**

**The Model:** This model is based on the similarity in preferences between two users and uses this to generate recommendations. The algorithm will generate an item similarity matrix of look-alikes for each movie that will be used to recommend look-alike movies to the user. For this similarity matrix we can use either a Jaccard Similarity, a Cosine Similarity or a Pearson Similarity.

**Why we are using it:** We are using Memory-Based Collaborative Filtering because of its ease of implementation and its quality of predictions. We are specifically using an Item-Item Collaborative Filtering instead of a User-User Collaborative Filtering model because it is much less resource intensive for when new users are added since the similarity matrix is built from the static movie list instead of the users. 

**Predicted Output:** The output is expected to be recommendations for a user based on the models predictions of what that user would rate the recommended movies by identifying what similar users have rated those movies.

**Evaluation:** We will use the Root Mean Squared Error (RMSE) metric to evaluate the accuracy of our predictions as this is a popular and standard metric.

**The Math:** There are three distance metrics used in the collaborative filtering in the comparison matrix:

**1. Jaccard Similarity:** Similarity is based on the number of users that have rated items A and B divided by the number of users who have rated either A or B. Jaccard similarity is commonly used when Boolean values are used instead of numeric ratings. 

**2. Cosine Similarity:** Similarity is the cosine of the angle between two vectors A and B. The closer the vectors are (the more they are related) the smaller the angle and larger the cosine coefficient is. The similarity coefficient falls between a value of [-1,1], where 1 shows a perfect relationship between sets A and B. The equation below is the dot product of the vectors A and B divided by their magnitude:

<div align="center">
  <img src="https://github.com/ByronKrauskopf/Group_3_Final_Project/blob/main/Resources/cosine_coeff.PNG" alt="cosine_coeff">
</div>

**3. Pearson Similarity (ρ):** Similarity is the Pearson coefficient between two vectors. The coefficient is the **product-moment** correlation coefficient and measures the linear correlation between two sets of data. Shown in the equation below, the coefficient is the ratio of the covariance of the two variables and the product of their standard deviations; the results are normalize  and will be a value between -1 and 1, with 1 being a perfect correlation.

<div align="center">
  <img src="https://github.com/ByronKrauskopf/Group_3_Final_Project/blob/main/Resources/pearson-similarity.png" alt="pearson_coeff">
</div>
  
The diagram below shows examples of scatter diagrams with different values of correlation coefficients (ρ):

<img src="https://github.com/ByronKrauskopf/Group_3_Final_Project/blob/main/Resources/scatter.PNG" alt="scatterplot">

The image below shows several sets of (x,y) points with their correlation coefficient between x and y. You can see below that the correlation reflects the strength and direction of the linear relationship (top row), but not the slope of that relationship (middle), or many aspects of nonlinear relationships (bottom). 

<div align="center">
  <img src="https://github.com/ByronKrauskopf/Group_3_Final_Project/blob/main/Resources/plot_1.PNG" alt="plot1">
</div>
  
More information can be found clicking on this [wiki](https://en.wikipedia.org/wiki/Pearson_correlation_coefficient) article here. 


<!--################Roadmap################-->
# Roadmap

The roadmap outlines the task's objectives, and expectations are introduced in a timetable structure utilizing an undertaking guide. Thus, the venture guide can be utilized to oversee partner assumptions and convey plans and direction assets.

Follow our roadmap below to implement our project according to the deliverables, named as segments from 1 to 4.

![](https://github.com/ByronKrauskopf/Group_3_Final_Project/blob/main/Resources/Capture2_%20Project%20Roadmap_Group3.PNG)

<p align="right">(<a href="#top">back to top</a>)</p>

<!--################Communication Protocol################-->

# Communications Protocol

General communication:
For this project all communications will be done via Slack for messaging and Zoom for meetings. Team members should check Slack at least once per day for any critical messages. 

Meetings:
Team meetings will occur 3 times a week on Tuesdays and Thursdays during class hours, and Saturday afternoons. Additional meetings can be scheduled through Slack as needed. 

Pull Requests:
When submitting a pull request in GitHub, the user should also post a notice in Slack so that all other team members are aware of the outstanding request in GitHub and can review and approve. All pull requests will require a minimum of 3 reviews and approvals from team members before merging.

<p align="right">(<a href="#top">back to top</a>)</p>

<!--################Contributors################-->

# Contributing
<div align="center">
  <a href="https://github.com/ByronKrauskopf/Group_3_Final_Project/graphs/contributors">
    <img src="https://contrib.rocks/image?repo=ByronKrauskopf/Group_3_Final_Project" />
  </a>
</div>

- Douglas Oliveira
- Omar Zu'bi
- Jathuson Jayakumar
- Danni Yang
- Byron Krauskopf


<p align="right">(<a href="#top">back to top</a>)</p>
