# Data Visualization in RStudio

## 1. Creating data frame and storing .csv files

To read .csv files in RStudio we need to make a dataframe and then store the .csv file to access it. To get a quick look into the table we can use head() which can help us retrieve the first 6 rows to give us an overview of the table. If you only want to retrieve the column names of the table we can use colnames()
 
![image](https://github.com/user-attachments/assets/9ad2ed4b-9348-4a67-994c-582f0aa4225c)

![image](https://github.com/user-attachments/assets/3711cbab-43ee-4d24-9268-7ead5cd428a1)

![image](https://github.com/user-attachments/assets/0987d7f3-9484-4531-81f9-eea49ea9ab69)

## 2. Creating a Plot

If we want to create any kind of visualization in RStudio we need to install the ggplot2 library before we go ahead. Listing down the functions used in the image below: 

1. ggplot2 is a system for declaratively creating graphics, based on The Grammar of Graphics. You provide the data, tell ggplot2 how to map variables to aesthetics, what graphical primitives to use, and it takes care of the details 
2. geom_point: 
The point geom is used to create scatterplots. The scatterplot is most useful for displaying the relationship between two continuous variables.

Note: The definitions were taken from the [website](https://ggplot2.tidyverse.org/)

![image](https://github.com/user-attachments/assets/e5f9c068-e106-4743-8d9d-c3ecb9cd61db)

![image](https://github.com/user-attachments/assets/4a87a64a-a698-424e-bda1-215d20a456fc)

## Exploring different Charts

Creating bar charts is of great help when we want to make use of filters. We can do that by showing each hotel type and market segment in the bar chart by using different colours to represent each segment. Listing down the functions with their definitions:

1. geom_bar: 
The bar geom is used to create bar charts. A barplot is used to display the relationship between a numeric and a categorical variable.

3. facet_wrap:
facet_wrap() wraps a 1d sequence of panels into 2d.

 ![image](https://github.com/user-attachments/assets/25d482e8-7724-400c-9cf5-e0748a91dbf8)

Once we have created the bar charts, we can see that it is not easy to compare the size of the market segments at the top of the bars. To solve this we can use the facet_wrap() to create a separate plot for each market segment to make our job easier to compare.

![image](https://github.com/user-attachments/assets/63639d00-8d5a-4e14-9ddb-43fc5f03288f)

The scenario mentioned below was a part of the hands-on activity given to us during our data analytics course and we were asked to solve it.

After considering all the data, your stakeholder decides to send the promotion to families that make online bookings for city hotels. The online segment is the fastest growing segment, and families tend to spend more at city hotels than other types of guests.
Your stakeholder asks if you can create a plot that shows the relationship between lead time and guests traveling with children for online bookings at city hotels. This will give her a better idea of the specific timing for the promotion.

Approach:
1) Filter the Data
2) Plot the filtered data

![image](https://github.com/user-attachments/assets/5fc221f2-d3d1-4688-9a8b-4cc90f7b8136)

![image](https://github.com/user-attachments/assets/32f5a435-3dfe-4c3b-a809-10f45a37fb2a)

There is also another way to do this by using the pipe operator (%\>%)

![image](https://github.com/user-attachments/assets/84bb643a-d0ec-4542-b3bf-5d356b4c7ea8)

![image](https://github.com/user-attachments/assets/a1616835-5b97-41d2-b208-a32897966100)

## Creating a scatter plot 

![image](https://github.com/user-attachments/assets/5aca0012-8559-4b9a-841d-25a09b5599f7)

![image](https://github.com/user-attachments/assets/6d0d7616-66ab-4847-9147-64032110ab60)

![image](https://github.com/user-attachments/assets/407e31cc-876b-4ef7-9824-433be3617c47)

Conclusion:
Based on your previous filter, this scatterplot shows data for online bookings for city hotels. The plot reveals that bookings with children tend to have a shorter lead time, and bookings with 3 children have a significantly shorter lead time (\<200 days). So, promotions targeting families can be made closer to the valid booking dates.
