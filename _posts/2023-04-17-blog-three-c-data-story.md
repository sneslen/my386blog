---
layout: post
title:  "Finding an Ideal Airbnb: A Data Story"
author: Sydney Neslen
description: "The final part to my data exploration of Airbnb"
image: /assets/images/airbnb3.jpg
---

## Summary

Airbnb is a popular website that connects potential hosts with travellers looking for a place to stay. [It was founded in 2007](https://news.airbnb.com/about-us/)! and has since grown to hold 6.6 million active listings, 4+ million hosts, and 100 thousand cities and towns that contain properties. However, it can be difficult to book a stay without accompanying difficulties such as low quality facilities, frustrating hosts, and unfulfilled expectations. So what are some promising factors that can indicate a good rental? I decided to explore some [properties in Utah](https://www.airbnb.com/utah-united-states/stays)! to see if there were any patterns to finding an ideal Airbnb. 

To start, I used the Python webscraping package, `BeautifulSoup`, to collect my data from the Airbnb website. This resulted in over 200 listings with 9 variables. I originally wanted to discover a relationship between pricing and any other variables, but there didn't seem to be much of an association other than number of bedspaces. I expected to find at least a couple of significant factors that affected pricing, especially rating score, but my efforts didn't seem to bear much fruit. 


## Results

Overall, there aren't many meaningful patterns present in this data. I decided to switch my focus to variables that affected ratings. I found that the most efficient and clear way to display my findings was in a correlation heatmap. The variables included are price, number of beds, rating, superhost status, number of reviews, and the length of the listing name. Ultimately, the most statistically significant correlation was between ratings and superhost status. There isn't much else of note when it comes to finding helpful indicators. 


<div style="text-align: center;">
<img src="https://raw.githubusercontent.com/sneslen/my386blog/main/assets/images/corr_heatmap.png" alt="" style="width:50%;"/> 
</div>


## Conclusion

Therefore, if we assume that rating scores are an accurate measure of quality of stay, the best way to find a good property is to check if the host is a superhost! Airbnb superhost status is granted when the host has an overall average rating of 4.8+ stars, has completed at least 10 stays, has less than a 1% cancellation rate, and has a 90% response rate. This finding definitely makes sense and shows that the superhost program is effective at identifying properties that are most likely reliable. Additionally, this data shows that paying more for a stay does not guarantee a better experience. This is good news in the sense that you can spend less but still have an enjoyable time. 

Thanks for following along with my data journey while I explore Airbnb listings! If you haven't read my past two posts on this dataset, make sure to check those out as well for additional context. 


### Link to repository
Here is a link to the [Airbnb repository](https://github.com/sneslen/airbnb.git)!