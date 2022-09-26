# Bikesharing
Created a data visualization story and dashboards for analysis of citi bike data using ETL methods in python to clean the data and Tableau for visualization.

## Resources
- `Software and Applications:`
  - Python
  - Jupyter Notebook
  - Pandas
  - Tableau Desktop
  - Tableau Public
  
## Project Overview:
The overview of this project incorporated a business proposal and pitch for citi bike for a particular group of potential investors. The goal and methodology of this project was to analyze the citi bike data that was collected in New York City on the month of August and launch a bike sharing business in Des Moines. The month of August was chosen specifically to analyze how the business operates in the peak of summer where tourisism is the highest. 
In order to convince and solidify the proposal to our potential investors that a bike-sharing program in Des Moines is profitable, we implemented on creating a bike trip analysis for one key stakeholder. For this analysis, we used Pandas to change the "tripduration" column from an integer to a datetime datatype. Then, using the converted datatype, we created an additional set of visualizations to:
- Show the length of time that bikes are checked out for all riders and genders
- Show the number of bike trips for all riders and genders for each hour of each day of the week
- Show the number of bike trips for each type of user and gender for each day of the week.

## Results 
For this part of the project, we created a story in Tableau and wrote our findings that describes the key outcomes of the NYC Citibike analysis:
#### `August Peak Hours`
![Screen Shot 2022-09-24 at 6 54 08 PM](https://user-images.githubusercontent.com/107281474/192124985-7d18233e-06f3-498b-817b-aa53650580b5.png)
During the most profitable month of the year which is August, in New York City in which the data was collected the most popular hours were between the hours of 5-6pm`(Hour of Starttime: 17-18)` with a count of over 200,000 rides and the hours of 8-9am`(Hour of Startime: 8-9)` with a count of over 140,000 rides. From the `August Peak Hours` horizontal bar chart, a trend that was uncovered is that people in New York City more than likely use the 
Citi Bike services to ride to and from their place of work as the typical working office hours fall within that timeframe. 

#### `Bike Utilization`
![Screen Shot 2022-09-24 at 7 13 08 PM](https://user-images.githubusercontent.com/107281474/192125321-48857212-2e3d-4dc2-8785-45cc7b6f2fc6.png)
Our potential investors were curious about the bike utilization during the month of August after our initial findings in the `August Peak Hours` sheet. We then created a packed bubbles visualization called `Bike Utilization` to show the utilization of each Citi Bike in New York City. We used the bike ID as a metric for determining which bikes have the highest utilization. Since we found the number of trips per bike during the month of August, we needed to figure out how long those rides are and if there are bikes that need more attention than others. The bubbles in this plot show the bike utilization levels. If a bike has a higher utilization level, it will be a larger bubble. In addition the bike ID has a color filter from Red to Blue to distinguish the bike.

#### `Checkout Time for Users`
![Screen Shot 2022-09-24 at 7 30 41 PM](https://user-images.githubusercontent.com/107281474/192174004-b91ebbf3-3460-41df-862c-0a0c8d8330be.png)
From our `Checkout Time for Users` dashboard, we visualized and graphed the length of time that bikes are checked out for all riders. in order to obtain this visualization, we:
- Add the number of records or the generated field that counts the number of records in the CSV file to the Rows.
- Add the "tripduration" column you converted to the Columns, and filter the "More" option by "Hour".
- Add the "tripduration" column again to the Columns, and filter the "More" option by "Minute", and then change the values from "discrete" to "continuous".
- Add the "tripduration" column that shows the "Hour" to the Filters field, and select "Show Filter".
- Edit the X and Y axis labels by right-clicking on the axis label and selecting "Edit Axis".
- Input the `Usertype Pie Chart` and `Count of 201908-citibike-tripdata.csv`
From the dashboard, nearly 81% of the Citi Bike users are subscribers, whereas 19% of that recorded demographic are customers that sometimes frequent the services of Citi Bike. As the visualization displays, user retention of Citi Bike is very high and any future business endavors or market openings should incorporate and highly advertise premium subscription incentives for subscribers and more features and benefits for customer conversion. In addition, the peak of minute of trip duration is 5 minutes inferring that customers use Citi Bike services for quick commutes.
