---
layout: post
title:  "Get the Best Bang for Your Buck: A Closer Look at airbnb Listings in Provo, UT"
author: Sydney Neslen
description: My process of scraping property listing data from the Airbnb website. 
image: /assets/images/airbnb.jpg
---
# Introduction
With the rise of short-term rentals in recent years, Airbnb has become a popular choice for travelers looking for unique and affordable accommodations. However, looking for a good quality property for a good price can be a daunting task. The good news is that by analyzing this dataset, we can gain insights into how different variables such as beds, reviews, and descriptions affect pricing. Whether you're looking to optimize your rental income or find the best deal on your next Airbnb stay, this information is very useful for anyone utilizing Airbnb.

# Description of the Process
I decided to do my analysis based on [Airbnb listings within Provo, UT](https://www.airbnb.com/s/Provo--Utah--United-States/).

On the page, there are 18 listings of potential properties to stay at. There are a total of 15 pages, which creates 270 total properties to obtain. From each listing, I collected the title, name, price, price unit (per night, etc), number of beds, rating, superhost status, and number of photos. 

To scrape a listing, I inspected the page and located the class tag to use to collect the rest of the data. 
![](/assets/images/inspect_airbnb.jpg)
  
From there, I identified the class tag for each element and used them to extract the data for each listing. 

The most difficult part was scraping all the listings from each page. I found the class tag for the "Next" button and using that link, gathered the data from the page and repeated the process. 

After that, I cleaned the data using `.get_text()` and `.strip()` to isolate the actual data. 


# Conclusion
My analysis of the Airbnb dataset will shed light on the various factors that impact pricing in the short-term rental market. By leveraging these insights, hosts can maximize their rental income while providing a competitive price for their guests. Similarly, travelers can use these findings to make informed decisions about their accommodations and find the best value for their budget. Ultimately, data analytics provides a powerful tool for both hosts and travelers to make the most out of the Airbnb platform. I hope this post has been informative and helpful in your own rental endeavors. Be sure to check back in where I perform further exploratory data analysis on this dataset!


# Link to repository
Here is a link to the [Airbnb repository](sneslen.github.io/airbnb/)!