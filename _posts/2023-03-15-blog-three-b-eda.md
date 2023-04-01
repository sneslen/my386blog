---
layout: post
title:  "Exploring Airbnb with Charts and Stuff"
author: Sydney Neslen
description: "Following my previous post, here is some exploratory data analysis on what a promising Airbnb property consists of."
image: /assets/images/airbnb2.jpg
---
# Introduction
Airbnb has revolutionized the travel industry by offering unique and affordable accommodations for travelers worldwide. With its popularity, there has been an explosion of Airbnb listings, making it difficult for both hosts and guests to determine the best price for their properties and stays. That's where exploratory data analysis (EDA) comes in. By analyzing a dataset consisting of data from [Airbnb listings in the state of Utah](https://www.airbnb.com/s/Utah--United-States/), we can uncover patterns and trends in pricing that can help hosts optimize their rental income and guests find the best deals on their next Airbnb stay. In this blog post, I will perform exploration on the dataset I previously scraped from the Airbnb website. Visit [my last blog post](https://sneslen.github.io/my386blog/2023/03/15/blog-three-a-repo.html) if you want to learn more about that process!


# On to the charts and stuff

The main focus of my analysis is factors that affect price. With this in mind, I constructed a few different graphs to see if I could identify any strong patterns or correlations. I compared different variables with price and created some scatterplots. 

This first one is price versus rating. it seems like there is a positive correlation between the two variables, but there is a wide spread. 
![1](/assets/images/price_rating.png)


I then compared number of beds with price. Again, the two factors seem to be related, but not strongly.
![2](/assets/images/beds_price.png)



This scatterplot consists of rating scores and number of reviews. I was curious if the number of reviews affected a property's score, and I was surprised to see that the more reviews, the higher the score. 
![3](/assets/images/rating_reviews.png)


This plot presents an average of ratings and prices by city. The larger the point, the more properties in that city. The cities with six or more properties are labelled. 
![4](/assets/images/price_rating_count.png)

![5](/assets/images/airbnb.jpg)

# Link to repository
Here is a link to the [Airbnb repository](sneslen.github.io/airbnb/)!