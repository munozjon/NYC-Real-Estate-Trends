# NYC-Real-Estate-Trends

For this project, we analyzed the real estate data out of New York City's most popular borough, Manhattan. Particularly, we analyzed the rental and sales data from before, during, and after COVID-19. Below is the analyses from each notebook, where the code and visualizations are found.

## Analysis of Manhattan Neighborhoods' Median Sales Prices
This Python notebook provides an analysis of median sales prices for Manhattan neighborhoods using data extracted from StreetEasy for the periods 2018-2022. The analysis aims to understand trends in median prices before, during, and after the COVID-19 pandemic.
Conclusion
The analysis reveals distinct trends in median sales prices across Manhattan neighborhoods. Before the onset of the COVID-19 pandemic in March 2020, median prices ranged from 0.6 to 1.4 million dollars. During the pandemic, there was a notable shift, with most areas experiencing a decline in median prices, except for the Upper West Side, which saw an increase. Post-pandemic, starting from 2021, there is a noticeable trend of increasing median prices across all areas, indicating a broader recovery and stabilization of the real estate market.
However, it's important to note some exceptions. Neighborhoods like Tribeca, Soho, and Midtown showed a continued decrease in values after the pandemic, suggesting localized market dynamics or shifts in demand. Additionally, some residents may have moved to other boroughs such as Queens or Brooklyn, impacting demand in certain neighborhoods.
Overall, the analysis highlights a complex interplay of factors influencing median sales prices, with neighborhoods showing distinct behavior. Notably, neighborhoods like Flatiron, Greenwich Village, West Village, and Chelsea showed significant increases in prices post-COVID, with some experiencing up to an 18% increase.

## Commercial Real Estate Trends
Do interest rates have an impact on the commercial real estate market?

Based on the data I obtained through open data resources in NYC. I was able to better understand the effect of Federal Reserve policy on the commercial real estate sector. Federal Reserve policy leading up to the beginning of COVID (March 2020), during COVID and the effects on our current economy by monetary policy.

Sales Volume: The lead up to the start of Covid showed weakness beginning to form in the commercial real estate sector. Sales volume decreased by 66% and bottomed out in 2020. The decrease in sales volume was a result of tighter monetary conditions from the Federal Reserve which raised interest rates and discontinued quantitative easing. The increase in total sales volume going into 2021 was a result of Federal Reserve policy u-turn during the drop in equity markets.The sales volume increase by 200% in that short period of time.The lowering of interest rates and purchases of CMBS lead to increased property sales for NYC commercial real estate.

Median Sales Price: The median sales price for all commercial buildings prior to 2020 was trending lower and bottomed out in 2020. The year of 2021 saw a sharp rise in the median sales price for the commercial real estate market.This was a result of many large commercial office buildings being sold during that time.The rise in the real estate during 2021 was a result of the lowering of the Fed Funds Rate and quantitative easing. The median sales price will continue to trend lower in the coming years from tighter monetary conditions and work environment transformations.

## Median Rental Pricings in Manhattn NYC, Pre and Post COVID-19
In this notebook I analyze the rental pricing pre and Post COVID-19 for most expensive city and borough in the world such as Manhattan in New York.

This notebook will attempt to answer: What is the most expensind neighborhoods to rent Manhattan,y, if any, while also examining if the COVID-19 period has affected the rental price? The notebook will utilize NYC rental data available on StreetEasy to attempt to answer the questions mentioned.

Some of the parameters set for this project include looking at data from the lfive six yefrom rs (January2018 December2022)

areaName is the name of the neighborhood, areaType is the setting oneighborhoodorhood, Borough is the New York county the neighborhood rewhile we have five Borough: Manhattan, Bronx, Brooklyn, Queens, staten Island for this project we analyse only Manhattan. s, and as mentioned, Price is the median rental price for that neighboations.
To explore the distribution of median rental pricing for each neighborhood, I used a violin plot, boxplot and histogram. From the first chart, we can see thatit is not normal distributed. One of main reason of big difference betweeen avarage rental prices is top neigborhood,those grafs we see below. We see standart deviation is 417As we know standart deviation is the avreage amount of variability in your dataset. It tells you, on average,how far each value lies from the mean. . 417$ standard deviation means that values are generally far from the mean.

If we analyse how prices changed during covide and after covid we see prices decrease durinc covid-19 for all neighborhood except top two neighborhood.From 2021 prices increased dramaticly for all neighborhood except last two neighborhood

An analysis of rental price trends reveals a notable decrease across most neighborhoods during the COVID-19 period. However, the top two neighborhoods experienced relatively stable prices. Subsequently, from 2021 onwards, there was a significant uptick in prices across all neighborhoods, except for the last two neighborhoods.

## Rental Inventory Analysis

### Introduction

My analysis is focused on the rental properties located in Manhattan, New York. With Manhattan being the most popular borough in New York City, it was appropriate to use its data as a way to analyze the rental inventory trends from before, during (03/2020 - 12/2020), and after the COVID-19 pandemic. In analyzing the rental inventory in the city, I sought to answer questions regarding the effect of the pandemic on inventory:

- Which neighborhoods, generally, see the most rental properties available?
- How did COVID affect available rental properties in Manhattan's neighborhoods?
- What trends were found in Manhattan's submarkets, and how did the pandemic affect these trends by quarter?

#### StreetEasy Dataset (https://streeteasy.com/blog/data-dashboard/[object%20Object])

For this notebook, I looked at the inventory of rental units in Manhattan from the years 2018 to 2022. The data was courtesy of StreetEasy, a website for housing and properties in New York City. It is known to be a reliable source for New Yorkers to find available housing, so they have access to data regarding the housing and rental market in New York City. In addition, their data is generally granular, with inventory statistics available by month, and by neighborhood or submarket, since 2010, and updated constantly. This allowed for my analysis to be reliable and allowed for trends to appear more meaningfully. The rental inventory is collected based on the number of rental listings available at any time during each month.


#### Maptiler API (https://docs.maptiler.com/cloud/api)

To represent each neighborhood's average inventory from 2018 to 2022 visually, I leveraged Maptiler's API reference to their Cloud Services to retrieve the latitudes and longitudes of each neighborhood in Manhattan. This free service allowed me to search for locations by name, so I was able to retrieve most of the neighborhoods' coordinates (while hard-coding the handful that were not found). With this, I was able to plot them onto a map of Manhattan, allowing for an interactive and engaging visualization of rental inventory in the city.

### Which neighborhoods, generally, see the most rental properties available?

Looking at the map of the neighborhoods' average inventory, we can see that there is a large number of rental units in the Upper East Side and Upper West Side, as well as Midtown Manhattan. The Upper East Side had an average of about 3,184 rental units in inventory between 2018 and 2022, while the Upper West Side had an average of about 2,753 units in inventory. This would generally suggest a higher demand for rental units in these areas of central Manhattan. In addition, there is a notably large number of neighborhoods in downtown Manhattan, making this submarket another popular area for people to rent.

### How did COVID affect available rental properties in Manhattan's neighborhoods?

The bar graph demonstrates the average inventory of each neighborhood from pre-COVID, during COVID, and post-COVID. As discussed prior, the areas with the most rental inventory include the Upper East Side and Upper West Side, Midtown, and neighborhoods in Downtown Manhattan. Prior to the pandemic, we can see that the average inventory for many of the neighborhoods was slightly greater than their inventory post-COVID, with a few exceptions. However, the most notable trend is how much more inventory was found during March to December of 2020, the beginning of the pandemic. We can see that pre-COVID, the Upper East Side's average rental inventory was 2,885 units, and that number jumped to 4,533 units during the start of COVID. We can see that, due to the pandemic, much fewer people began to rent units in Manhattan. This would then lead to a massive jump in inventory as shown for almost every neighborhood in the dataset. With fewer people wanting to move into the congested areas of manhattan, it is expected that rental units would be more prolific as a result.

Moving forward, another interesting trend is the average rental units during COVID and post-COVID, from 2021 to 2022. Again, in the Upper East Side, the average inventory post-COVID was about 2,885 units, a large drop from the 4,533 during COVID. A drop is found in most other neighborhoods, including the Upper West Side, parts of Midtown, and Chelsea. Furthermore, while it appears the average units post-COVID are generally at the same level as the average units pre-COVID, there is a notable discrepancy between the two time periods. We will explore this more in the next section.

### What trends were found in Manhattan's submarkets, and how did the pandemic affect these trends by quarter?

Analyzing the average inventory by quarter, we can see many trends. Taking a look at each submarket, we see that Downtown Manhattan has the highest average inventory of all submarkets in the borough. Downtown Manhattan has the most neighborhoods, which would likely explain the average inventory being greater than the others. While the Upper East Side was among the largest neighborhoods in average inventory, it sits below all of Midtown and all Downtown neighborhoods. Meanwhile, all Upper Manhattan is among the lowest in average inventory, which coincides with an earlier trend discussed that areas near central Manhattan (such as Midtown) see more inventory due to a greater demand for people to rent there.

Upon analyzing the trends over each quarter, we can see that between Q4 and Q1 there is a dip in inventory, especially prior to the pandemic. This is likely due to people who moved into these rental units in previous quarters, leading to fewer rental units available as they are occupied. This is further backed by the peaks found in Q2 and Q3, as people look to renew their lease or find another available rental unit. This trend happens in all submarkets, most notably in Downtown Manhattan where the average rental inventory for Q4 2018 was about 5,300, while Q2 2019 saw that number increase to about 7,322.

Moving forward, the average inventory during the pandemic had a notably large spike, particularly in Q3 of 2020. We can see that, from Q1 of 2020, the average inventory for each submarket was trending upward and peaked in Q3, before beginning to fall in Q4 and into 2021. As discussed previously, the pandemic led to many people not wanting to rent in Manhattan. Seeing as how Q2 and Q3 were typically months where inventory would be highest, the inventory grew much bigger as people decided not to renew their lease and/or move elsewhere. In Downtown Manhattan, the average rental inventory was about 15,603 units in Q3 of 2020, over three times as many as there was in Q1 of 2020 (4,559 units).

In the years since COVID, the average inventory began to fall. For all of 2021, most of the submarkets (except for Upper Manhattan) continuously dropped in rental units available, before beginning to rise again in Q2 and Q3 of 2022. Q4 of 2021 saw the lowest drop of the dataset for many of the submarkets; Downtown Manhattan had an average inventory of about 3,416 units. However, the peak inventory averages of 2022 was notably less than the peaks found in 2018 and 2019, before COVID. For example, in Downtown Manhattan, a Q2 2022 average of 5,087 units or a Q3 average of 5,821 units is much less than the 7,716 average units seen in Q2 2019. The overall decrease in available inventory in the years since COVID suggest people either renewing their leases more often (meaning their unit would not be put on the market), or just a general decline in available rental units.