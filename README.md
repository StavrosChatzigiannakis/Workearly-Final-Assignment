# Workearly-Final-Assignment

Workearly Final Assignment by Stavros Chatzigiannakis

At first we review the data on the database level :

First we have to load up our data on MySQL workbench to see what is the quality 
and the formatting of our information. We can see clearly that we need to format our geo 
location since Tableau wont be able to detect that kind of formatting. So our next move is
to grab the data that we need and that is all from 2016 - 2019. We then sort our data by date 
and then export it to .csv file format.

Secondly we read our data using Python and make the necessary transformations and calculations.
 1) Zip Code must converted to a integer from a float.
 2) Coordinates must be reformatted to seperate columns each representing Latitude and Longtitude respectively.
 3) We can calculate each sale's profit by doing this column-wide calculation ((state_bottle_retail-state_bottle_cost)*bottles_sold).
 4) Then it is time to find the Most Popular item per zip_code using groupby.
 5) And last we can calculate each store's Percentage of Sales by doing column-wide calculations.
 6) Exporting to .csv .

After , we can insert our data sources to Tableau and start managing relations betweeen tables as well as the data type of each of the 
columns. Following that we can design the two necessary components of our Dashboard which are Most Popular Items by Zip Code and
Percentage of Sales per Store. We can use the simplicity to read of a Treemap instead of a regular Pie Chart for our Percentages 
and a Simple Map for the Zip Code. Then we can create two more Graphs to add to the granularity of our Dashboard by creating insights 
of our Most Profitable Items and Most Profitable Stores using the measure which we calculated on Python.


