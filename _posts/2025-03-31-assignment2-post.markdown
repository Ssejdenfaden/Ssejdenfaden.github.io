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

![Assault crime over the years 2003-2025 in San Fransisco](/assets/calplot-assignment2-5.png)

When we take a look at the time series data for assault specificly, we see a few interesting trends.

Firstly, in the vast majority of the years, January 1st appears to have a high count of assault crimes compared to the remainder of the year. We could speculate that this is due to New Years celebrations, but interestingly December 31st does not seem to be particularly high in assault charges, meaning they are kept to after the new year has arrived. Another big celebration day in the US is 4th of July, however, that one doesn't seem to have as strong a trend of assault crimes. This may speak to a difference in the type of celebration; the 4th of July is more often celebrated with family and is held earlier in the day compared to New Years celebrations. Another holiday that is perhaps a bit more similar in its celebrations compared to New Years, at least for young adults and particularly college students, is Halloween on the 31st of October; here we do see a spike in assault crimes on the 31st of October and 1st of November some years, however, still not as consistently as the New Years celebrations. We tried to look for news regarding January 1st, 2003, as this date seems to have a particularly high number of assault cases, however, we were unable to find anything.

Secondly, we see that in general, the number of assault crime occurences seem to be dwindeling as the years progresses. This consistent with what we saw for prostitution crimes in the previous assignment. This may either be due to a genuine decrease in such crimes over the years possibly due to it becoming more difficult to do so or more socially taboo (although we would think assault generally has been seen as the same amount of taboo in recent time), or, it can be due to less policing or less reporting from civilians, the latter potentially due to less trust in the police. With our current data, it is difficult to say which of these it may be, but it is clear that something has been happening incrementially over the years.

## Comparing assault crime with other types of crimes over the years

<iframe src="/assets/bokeh_plot_monthly-2.html" width="800" height="600" frameborder="0"></iframe>

The monthly distribution of to 5 focus crimes: Assault, Vehicle Theft, Vandalism, Drug/Narcotic, Laurency/Theft in San Francisco from 2003 to 2025 highlights the consistent nature of this crime across all months. Among all the crimes, LARCENY/THEFT is the most accured crime. The highest laurecy crime incidents recorded in June due to public activity, tourism, while the absence of this crime in December due to seasonal changes.
Drug crime is on the 5th place, where these incidents are accured with seasonality from April to December.
As From January to March corresponds to winter season and mostly people avoide outdoor activities and community driven events explains the absesnce of this crime.

Assault is the 2nd highest crime accured  with 1030 incidents. And it is also accured in all months and almsot all days of the week due to it's nature as crime that happens in various sistuations, such as personal disputes, conflicts in public places likely to occur in densely populated urban areas where interpersonal interactions are frequent. This explains why the crime occured in all months.

Assaults are often linked to alcohol or drug use, which can occur at any time of the year or day. Economic hardships or unemployment can lead to increased stress and conflicts, contributing to assault incidents.

From the hourly distribution analysis of assault crimes it accured almost all the day except early morning hours. This could be due to the transition period when people just wake up and travel to work and doing morning activities. The assault crime recorded high at afternoon 12 and from evening to midnight recorded highest may be due to alchahol consumption etc.
 
To conclude, Unlike other crimes that show seasonal trends, assault is influenced by human behavior, social interactions, and environmental factors. Addressing the root causes, such as alcohol abuse, economic stress, and interpersonal conflicts, can help reduce the frequency of assault crimes and improve public safety.

## References
1. Police Department Incident Reports Historical 2003: https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-Historical-2003/tmnf-yvry/about_data
2. Police Department Incident Reports 2018 to present: https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783/about_data
3. Earthquake shakes San Fransisco area: https://eu.usatoday.com/story/news/nation/2018/01/04/earthquake-shakes-san-francisco-area/1002768001/ 
4. Top Stories of 2018 on ABC7News.com (San Fransisco): https://abc7news.com/year-in-review-2018-abc7-top-stories-news-of-the/4939013/ 

## Contributions
__Shirisha:__ Bokeh graph and anaylsis

__Agathe:__ Map graph and analysis

__Simone:__ Time Series graph and anaylsis