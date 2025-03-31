---
layout: post
title:  "Assignment 2: Assault crime in San Fransisco"
date:   2025-03-31 12:12:27 +0100
categories: assignments
---
_By group 12: Agathe d'Aubenton-Carafa (s243230), Shireesha Myadari (s190030), and Simone Sejdenfaden (s241647)_


In this assignment we are looking at San Fransisco crime data over the years 2003-2025. The data is from DataSF, a citywide government project providing open source data pertaining to the city. The data was originally split into two datasets, [2003-2018](https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-Historical-2003/tmnf-yvry/about_data) and [2018-present](https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783/about_data) which we combined and pre-prossesed, ensuring cohesiveness of the data. For example, irrelevant columns were dropped, categories were were updated to be the same name across the datsets, and column names were changed to be the same across the datasets as well. For our analysis we chose to focus on assault crime data as we found this to have some interesting insights and a rather large amount of data. It should be noted that we are utilizing the full range of years (2003-2025) as this was specified in assignment 1 and no changes in this specification was noted for assignment 2.

## Assault crime occurences in San Fransisco over time
To start, we will be looking at assault crime occurences in San Fransisco over the years. To more easily see if any temporal trends appear, we will be making a calendar plot. This allows us to easily find patterns in the data.

![Assault crime over the years 2003-2025 in San Fransisco](/assets/calplot-assignment2-4.png)

When we take a look at the time series data for assault specificly, we see a few interesting trends.

Firstly, in the vast majority of the years, January 1st appears to have a high count of assault crimes compared to the remainder of the year. We could speculate that this is due to New Years celebrations, but interestingly December 31st does not seem to be particularly high in assault charges, meaning they are kept to after the new year has arrived. Another big celebration day in the US is 4th of July, however, that one doesn't seem to have as strong a trend of assault crimes. This may speak to a difference in the type of celebration; the 4th of July is more often celebrated with family and is held earlier in the day compared to New Years celebrations. Another holiday that is perhaps a bit more similar in its celebrations compared to New Years, at least for young adults and particularly college students, is Halloween on the 31st of October; here we do see a spike in assault crimes on the 31st of October and 1st of November some years, however, still not as consistently as the New Years celebrations.

Another very peculiar trend we are seeing, is the first 4.5 months of 2018; here we consistently see a significantly higher amount of assault crimes compared to both the rest of the year and the other years as well. While many events happened that year, from an [earthquake on January 4th](https://eu.usatoday.com/story/news/nation/2018/01/04/earthquake-shakes-san-francisco-area/1002768001/) to [cannabis becoming legal](https://abc7news.com/year-in-review-2018-abc7-top-stories-news-of-the/4939013/), none of these events seem to warrant the huge spike in assault crimes. We were furthermore unable to find any information on a possible police effort or increased police presence. This leads us to suspect there may be an error in or processing of the data; since 2018 was the cutoff year for the two crime data sets, perhaps there is a possibility some crimes have been double counted? However, checking our data (a subset seen below), there does not seem to be enough supposedly duplicate data (45 rows have been flagged as such). As such, it is diifuclt for us to determine what the cause of this spike is.

![Duplicates in data January to April 2018](/assets/duplicates.png)

Finally, we see that in general, the number of assault crime occurences seem to be dwindeling as the years progresses. This consistent with what we saw for prostitution crimes in the previous assignment. This may either be due to a genuine decrease in such crimes over the years possibly due to it becoming more difficult to do so or more socially taboo (although we would think assault generally has been seen as the same amount of taboo in recent time), or, it can be due to less policing or less reporting from civilians, the latter potentially due to less trust in the police. With our current data, it is difficult to say which of these it may be, but it is clear that something has been happening incrementially over the years.

## References
1. Police Department Incident Reports Historical 2003: https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-Historical-2003/tmnf-yvry/about_data
2. Police Department Incident Reports 2018 to present: https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783/about_data
3. Earthquake shakes San Fransisco area: https://eu.usatoday.com/story/news/nation/2018/01/04/earthquake-shakes-san-francisco-area/1002768001/ 
4. Top Stories of 2018 on ABC7News.com (San Fransisco): https://abc7news.com/year-in-review-2018-abc7-top-stories-news-of-the/4939013/ 

## Contributions
__Shirisha:__ Bookeh graph and anaylsis

__Agathe:__ Map graph and analysis

__Simone:__ Time Series graph and anaylsis