# sqlalchemy-challenge

This challenge analyzes data around Hawaiian Rainfall levels to help inform the best time of year to travel to Honolulu, Hawaii. Data available locally via CSV (in "Resources" folder) is compiled and organized via SQL in a SQLite file, allowing us to bridge the gap between the CSV and Python.

**Climate Analysis**
As a first step in this challenge, we use the SQLite file to visualize the daily rainfall data from 9 different stations in Hawaii across 2021 instances between 8/23/2016-8/23/2017.
The average daily rainfall across these stations is .18 inches/day, but up to 6.7 inches has been recorded in one day. The Station with the most rain recorded was USC00519281, and the station with the least was USC00518838; Knowing this, vacationing near the USC00518838 station may help improve our chances of avoiding rain during our trip.

According to the data, May through July historically have seen the lowest daily precipitation levels, while winter, especially January through April, tends to see the most rain. In the most active station, we can see that rainfall tends to dropoff on days where the temperature is >80 degrees, and peaks around 75-78 degrees, further supporting that we should plan our vacation in the summer months. 

**Flask API**
The second step of the challenge was to publish our SQLite findings into a custom API connection through Flask. This will allow users to check historical rainfall levels across different stations and dates.
To utilize the API, run the flask_app_jw.py file in Terminal/GitBash and follow the HTTP Provided: (Example message: * Running on http://127.0.0.1:5000)

Once on the site, you can link to different APIs or type the date you desire using the URL extension in the MMDDYYYY format
