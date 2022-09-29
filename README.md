# surfs_up
Precipitation and Weather Station analysis using the following:
- Python
- Jupyter Notebooks
- SQLite
- SQLAlchemy
- Flask
## Overview of Surfs Up Analysis
In order to convince an investor to open up a shop in Oahu, Hawaii under the name ***Surf n' Shake***, an analysis had to be conducted on a dataset, this analysis would provide a clear idea on the weather conditions of this region and how suitable it would be to invest in such a shop given the results.

This data was stored in an **SQLite** database, to connect to this database and preform queries, **SQLAlchemy** was used.
The set of dependencies that were used for this project could be viewed in the following screenshot:
![dependencies]()
In order to have the results easily accessed by people who are less familiar with coding, we opted to create a webpage using routes via **Flask** and running it.
![flaskapp]()
![webpage]()

## Results
First thing we did manipulating the data, we looked at 2021 observations of precipitation throught 365 days from August 23, 2016 (first day W. Avy's went surfing and had icecream at the same day) to August 23, 2017:
![yearresults]()
![precip_graph]()
above results show that indeed Ohua is a very sunny region in general, throught the mentioned 365days there was an average of only 17.7% of precipation.
After looking at precipitation, we obseved how many stations were gathering the data and which one provides the most data points, we found that there was a total of 9 stations, with the station **USC00519281** providing a max of 2772 measurements and the station **USC00518838** providing a minimum of 511 measurements.
![station]()
## Results of the challenge
In the challenge we looked at the statistics of the temperature in the months of June and December, and I added two additional queries for the precipation at these two particular months as well:
- temprature:
![junetemps]()
![dectemps]()
- precipitation:
![juneprec]()
![decprec]()
From the descriptive statistics above, we can see that there is an average precipation of 22 inches for the month of December and 13.6 inches for the month of June, we can also observe that the latter is almost 4&deg;F hotter than December with an average temperature of 75&deg;F, while December has an average temperature of 71&deg;F.
We can also observe that for both months 50% of the time, the temperature is above 70&deg;.
The data also states that there isn't any big fluctuation neither in Temperature nor Precipitation, the weather is fairly stable and pretty sunny.

## Summary
The data shows that Oahu is a suitable region for a surfing and ice cream business, as the rainfall throughout the year is light and there isn't any drastic change in temperature or precipitation, the region is sunny and perfect for people to go to the beach to surf and enjoy ice cream most days of the year. The investor should invest in opening the Surf n' Shake shop.
To further analyse the weather we could gather data on wind for example, as it is a key parameter in Surfing.
