
## Introduction
A Movie recommender system has became an interesting research topic due to the growth of users in a mobile environment. To recommend movies, a complete aggregation of user’s preferences and reviews are required to assist users to find the best movies in a more convenient way.

---
## Features 📋
* Existing users can login and new users can register.
* Users can search through various movies.
* Users can submit ratings for the movies.
* Users can add movies to their watch list(My List).
* Users can get movie recommendations (Recommendation algorithm named Collaborative Filtering is used which suggests new movies based on the ratings given by the user.)
---

## Technologies used 
* Python (Jupyter Notebook) 
* Web Technologies- html,css,javascript, bootstrap, Django
* Machine learning libraries in python3- pandas,numpy,scipy
* Database used- SQLite

---

## Algorithm Used- Collabortive Filtering 
* Collaborative filtering filters information by using the interactions and data collected by the system from other users. It's based on the idea that people who agreed in their evaluation of certain items are likely to agree again in the future.
* When we want to find a new movie to watch we'll often refer our friends for recommendations. Naturally, we have greater trust in the recommendations from friends who share tastes similar to our own.
* Collaborative-filtering systems focus on the relationship between users and items. The similarity of items is determined by the similarity of the ratings of those items by the users who have rated both items.
* There are two types of collaborative filtering
    * **User-based**- which measures the similarity between target users and other users.
    * **Item-based**- which measures the similarity between the items that target users rate or interact with and other items.
   
> I have used user based collaborative filtering in this project.

> In this project, Slope One algorithm is used in order to predict individual recommendations, which are further  combined into a group recommendation using the multiplicative utilitarian strategy. Slope one algorithm is a special form of collaborative filtering algorithm, which has the characteristics of easy to use, accurate recommendation and high computational efficiency. We have chosen a Group Model Based approach in order to implement a group recommendation strategy, by building the group profile using the individual profile of each member of the group. With this approach, a group recommender system considers the preferences of each individual in the group with some criterion that maximizes the happiness of the group (also called group’s satisfaction). The concept of group happiness can vary, it sometimes corresponds to the average of preferences of the members, and other times to the happiest (and least happy) member, etc.
---

## Problems faced and solutions adopted to resolve them
* Ramp-Up and Cold Start problems
* slope one algorithm can lead to ramp-up and cold start problems.
* To solve these problems an initial load is made using the MovieLens 10M dataset with data from anonymous users, items and scores. Once this dataset is loaded, we       use this data to initialize the matrix of average of rating differences used by the Slope One algorithm. 
* Thus, taking advantage of the benefits of the Slope One algorithm, new users must just rate a few movies when they enter the system for the first time so that the     algorithm can find entries in the matrix of average of rating differences and start generating good recommendations for the user.
   
## Web Application Development
* Register page(for new users)

![image](https://user-images.githubusercontent.com/106422898/170814273-4cd452de-022d-45f5-854c-5f14e12b2f18.jpeg)


* Login Page(for existing users)

![image](https://user-images.githubusercontent.com/106422898/170814304-2aed9f01-cf2d-4842-824e-34699c6b1824.jpeg)


* Browse through movies

![image](https://user-images.githubusercontent.com/106422898/170814310-346b5276-2d6f-4671-9c11-ebed43f77a9e.jpeg)

* My List

![image](https://user-images.githubusercontent.com/106422898/170814324-68cfc010-021a-4481-8a89-4add299e15fa.jpeg)


* Get Recommendations

![image](https://user-images.githubusercontent.com/106422898/170814328-8a6c78c6-ad20-45b7-ba39-365adb3359a7.jpeg)


## Installation 📦

* Clone the project and download the source code.
* Once inside the folder run following commands:

> $ pip install -r requirements.txt                                                                                           

> $ python manage.py runserver

NOTE: Run server locally
    : Install Python 3.7 to run the source code 

Go to > localhost:8000

     
 
