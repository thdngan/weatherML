# weatherML
Soooo i did this little project following the instructions from the [Predict The Weather with Machine Learning](https://www.youtube.com/watch?v=km95-NMT6lU&t=2102s&ab_channel=Dataquest) project from Dataquest.

I looked for the weather data from Hanoi, where I currently stay, to make it more relatable and see if I can make it useful. Several changes were made to suit the data available.

Near the end of the project, I encountered an error where it said I "cannot reindex on an axis with duplicate labels". So basically, I was trying to  create another column to calculate the monthly average temperature from the maximum temperature column, grouping the rows together according to the months. But turns out there are duplicated values in this column.

I used df.index.is_unique and df.index.duplicated() to identify and look for these duplicated values and eventually found out that all the data that I first downloaded from NOAA were already non-unique LOL.

So I guess I either need to deal with these values by removing them (but they make up most of the data lol) or I need to find data from other sources.
