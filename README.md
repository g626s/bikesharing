# Bikesharing
Created a data visualization story and dashboards for analysis of citi bike data using ETL methods in python to clean the data and Tableau for visualization.

## Resources:
- `Software and Applications:`
  - Python
  - Jupyter Notebook
  - Pandas
  - Tableau Desktop
  - Tableau Public
  
## Project Overview:
The overview of this project incorporated a business proposal and pitch for Citi Bike for a particular group of potential investors. The goal and methodology of this project was to analyze the Citi Bike data that was collected in New York City on the month of August and launch a bike sharing business in Des Moines. The month of August was chosen specifically to analyze how the business operates in the peak of summer where tourisism is the highest. 
In order to convince and solidify the proposal to our potential investors that a bike-sharing program in Des Moines is profitable, we implemented on creating a bike trip analysis for one key stakeholder. For this analysis, we used Pandas to change the "tripduration" column from an integer to a datetime datatype. Then, using the converted datatype, we created an additional set of visualizations to:
- Show the length of time that bikes are checked out for all riders and genders
- Show the number of bike trips for all riders and genders for each hour of each day of the week
- Show the number of bike trips for each type of user and gender for each day of the week.

## Results:
For this part of the project, we created a story in Tableau and wrote our findings that describes the key outcomes of the NYC Citibike analysis:
#### `August Peak Hours`
![Screen Shot 2022-09-24 at 6 54 08 PM](https://user-images.githubusercontent.com/107281474/192124985-7d18233e-06f3-498b-817b-aa53650580b5.png)
During the most profitable month of the year which is August, in New York City in which the data was collected, the most popular hours were between 5-6pm`(Hour of Starttime: 17-18)` with a count of over 200,000 rides and the hours of 8-9am`(Hour of Startime: 8-9)` with a count of over 140,000 rides. From the `August Peak Hours` horizontal bar chart, a trend that was uncovered is that people in New York City more than likely use the 
Citi Bike services to ride to and from their place of work as the typical working office hours fall within that timeframe. 

#### `Bike Utilization`
![Screen Shot 2022-09-24 at 7 13 08 PM](https://user-images.githubusercontent.com/107281474/192125321-48857212-2e3d-4dc2-8785-45cc7b6f2fc6.png)
Our potential investors were curious about the bike utilization during the month of August after our initial findings in the `August Peak Hours` sheet. We then created a packed bubbles visualization called `Bike Utilization` to show the utilization of each Citi Bike in New York City. We used the bike ID as a metric for determining which bikes have the highest utilization. Since we found the number of trips per bike during the month of August, we needed to figure out how long those rides are and if there are bikes that need more attention than others. The bubbles in this plot show the bike utilization levels. If a bike has a higher utilization level, it will be a larger bubble. In addition the bike ID has a color filter from Red to Blue to distinguish the bike data.

#### `Checkout Time for Users`
![Screen Shot 2022-09-24 at 7 30 41 PM](https://user-images.githubusercontent.com/107281474/192174004-b91ebbf3-3460-41df-862c-0a0c8d8330be.png)
From our `Checkout Time for Users` dashboard, we visualized and graphed the length of time that bikes are checked out for all riders. In order to obtain this visualization, we:
- Add the number of records or the generated field that counts the number of records in the CSV file to the Rows.
- Add the "tripduration" column you converted to the Columns, and filter the "More" option by "Hour".
- Add the "tripduration" column again to the Columns, and filter the "More" option by "Minute", and then change the values from "discrete" to "continuous".
- Add the "tripduration" column that shows the "Hour" to the Filters field, and select "Show Filter".
- Edit the X and Y axis labels by right-clicking on the axis label and selecting "Edit Axis".
- Input the `Usertype Pie Chart` and `Count of 201908-citibike-tripdata.csv`

From the dashboard, nearly 81% of the Citi Bike users are subscribers, whereas 19% of that recorded demographic are customers that sometimes frequent the services of Citi Bike. As the visualization displays, user retention of Citi Bike is very high and any future business endeavors or market openings should incorporate and highly advertise premium subscription incentives for subscribers and more features and benefits for customer conversion. In addition, the peak of minute of trip duration is 5 minutes inferring that customers use Citi Bike services for rather quick commutes.

#### `Checkout Times By Gender`
![Screen Shot 2022-09-24 at 7 31 01 PM](https://user-images.githubusercontent.com/107281474/192174788-1e83c376-8dd7-444f-b21d-1170e56570d8.png)
In this visualization, we graphed the length of time that bikes are checked out for each gender. In order to obtain this visualization we:
- Repeated steps 1-4 of the `Checkout Times for Users` visualization.
- Add the converted column for gender as a color to the Marks field, add it to the Filters field, and select "Show Filter".
- Edit the X and Y axis labels by right-clicking on the axis label and selecting "Edit Axis".

From the previous visualization, the checkout time trend between genders falls within the same timeframe and slope pattern. In the male category however, there is a massive slope and count of male riders than female and "unknown" customers. Although there are many customers who decide to not say their gender, the collection of data should have implemented more inclusive answer selection to better understand the trip duration data. 

#### `Trips by Weekday Per Hour`
![Screen Shot 2022-09-25 at 6 14 17 PM](https://user-images.githubusercontent.com/107281474/192175961-47541f6a-3624-4f1f-ae53-d6f3db34319e.png)
In this visualization, we graphed the number of bike trips by weekday for each hour of the day as a heatmap. In order to obtain this heatmap visualization we:
- Add the "Starttime" column to the Rows, and filter the "More" option by "Hour".
- Add the "Stoptime" column to the Columns, and filter the “More” option by "Weekday".
- Add the number of records or the generated field that counts the number of records in the CSV file to the Marks field as a color. Select "Automatic" for the type of graph to create the heatmap.
- Format the Y axis of the Starttime by Hour to show the 12-hour format.

From the visualization of the heatmap, it helps support the previous visualiztion `August Peak Hours` in that the concentration on the count of rides falls between the popular times during working office hours and days with the interesting exception of Wednesdays. Furthermore, Saturdays have the most centralized heat mapping in the afternoons and implementing a ride sharing discount or policy can help further increase revenue or product exposure in the target area. 

#### `Trips by Gender (Weekday Per Hour)`
![Screen Shot 2022-09-25 at 6 30 51 PM](https://user-images.githubusercontent.com/107281474/192183108-a2a6c91d-7377-40bc-82ce-f5a5e5ff43ef.png)
In this visualization, we graphed the number of bike trips by gender for each hour of each day of the week as a heatmap. In order to obtain this, we:
- Repeat steps 1-3 from the "Trips by Weekday per Hour" visualization.
- Add the converted column for "Gender" to the Columns and to the Filters field, and select "Show Filter".
- Format the Y axis of the Starttime by Hour to show the 12-hour format.

From the visualization of the heatmap, the heatmap supports the `Checkout Times By Gender` visualization in which the trip duration time and trend by gender is apparent by the density of the color in the same time frames. 

#### `User Trips By Gender By Weekday`
![Screen Shot 2022-09-25 at 7 43 12 PM](https://user-images.githubusercontent.com/107281474/192183706-096d7ff4-7b9d-4444-8717-05267a7bf2a9.png)
In this visualization, we created a heatmap that shows the number of bike trips broken down by gender for each day of the week by each Usertype. In order to obtain this heatmap, we:
- Add the converted column for "Gender" to the Columns and to the Filters field, and select "Show Filter".
- Add the "Usertype" to the Rows and to the Filters field, and select "Show Filter".
- Add the "Starttime" column to the Rows, and filter the "More" option by "Weekday".
- Add the number of records or the generated field that counts the number of records in the CSV file to the Marks field as a color. Select "Automatic" for the type of graph to create the heatmap.

In correlation to the `User Type Breakdown` pie chart, the heatmap nearly visualizes the exact same data trend and behavior of number of subscribers of Citi Bike based on gender in which male subscribers are the most dominant compared ti female subscribers as well as customers. 

## Summary:
With the given Citi bike dataset, to help further analyze and help our potential investors reach a conclusion, we would recommend on creating two additional visualizations for further analysis and strategy. It would be imperitive and vital to know and observe the Citi Bike customers and subscribers by age as well as income. This would be done by implementing Tableau's calculated field to use date of birth to get the age of each count of rider in the dataset as well as creating another parameter to visualize income. Lastly, another metric that could be used to analyze the data is converting the activity into measurable categories to draw subscription and product strategies to many target markets.

## Tableau Public Link
View the Tableau Public Story here:

[link to dashboard](https://public.tableau.com/app/profile/gustavo.sanchez8211/viz/CitibikeBusinessProposal/CitibikeBusinessProposal)
