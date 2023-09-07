# Temperature prediction with Machine Learning
Soooo i did this little project using the weather data from Hanoi, where I currently stay, to predict the temperature using Machine Learning.

I ran into an error near the end of the project that said I "can not reindex on an axis with duplicate labels." So, basically, I was attempting to build another column to determine the monthly average temperature from the maximum temperature column, while grouping the rows by months. However, it turns out that there are duplicate values in this column.

I used df.index.is unique and df.index.duplicated() to identify and search for duplicated values, and eventually discovered that all of the data I first downloaded from NOAA were already non-unique LOL.

So I think I'll have to deal with these values by removing them (though they make up the majority of the data, lol) or find data from other sources.

I'm currently still trying to resolve this and also continue adding my own analysis and interpretations for optimization.
