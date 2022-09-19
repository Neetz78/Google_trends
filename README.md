# Google_trends Data Collection TTA

### Code TTA assesstment: To retrive weekly and daily google trends data from 2015-01-01 to present.


## Idea:

I chose to use Pytrends API to retrieve google trends data as it is open source and performs well enough to capture the data that we are aiming for.

## the amount of time you spent on finishing the program code (or pseudo code),

I took about half a day to complete this entire code.Main reason being it took time to analyze how to retrieve weekly data for more than 5 years old.

## the different ways you have tried to approach the TECH ASSESSMENT, 

The different approaches I went with this assessment is mainly for capturing weekly data, 
* First I chose to retrieve data all together from 2015, once captured I noticed that the data collected is in months and we do not see weekly capture of data.
* Second I decided to first capture weekly data for the past five years using the function I designed get_weekly_data by passing bitcoin as a keyword parameter. The data collected is for Canada region which can be changed by setting the geo parameter to desired location.
* Once done with past five years,I coded another function to retrieve weekly data from 2015 to 2018, which causes overlap for the last few months of the 2017 year with the five years data.
* I programmed another function to combine these two dataframe into a single one by removing the duplicates and added steps to call the other two functions within this function, so all one has to do is call this function and a final weekly dataset is obtained for the keyword bitcoin from 2015 to present.

## the reasons of settling on the current approach, and finally, 
 Reason for settling on this approach is the api is open source, and have tons of research material .If I run to any problems or need to scale my code in future it would be easier to find materials.
 
## how to execute your program.
Run the below functions  to obtain weekly and daily data

* final_weekly_data(['bitcoin'])
* get_daily_data(['bitcoin'])
