# Which Customers Spend the Most? Segmenting Brazilian Delivery Platform Users
Understanding which customer segment bring in the most value is a key question for any company, especially in the competitive world of tech-based delivery services. For this project, I analysed customer data from a Brazilian delivery platform case study in Kaggle, aiming to find out which age and income groups spend the most, and how their purchasing behaviour could help shape the company’s marketing strategy. 

This analysis was completed as part of the #### [Data Analytics Accelerator Bootcamp](https://datacareerjumpstart.com/bootcamp). The main goal is to help the company's stakeholders decide which customer segment to focus on, and to support the creation of a clear positioning statement. By identifying the most valuable segments, the company can make better decisions about where to direct its marketing efforts.

Market Segmentation is when you divide the market into groups that share similar characteristics such as age, income, purchasing behaviour, and product preferences. Targeting is when you choose to focus your marketing efforts on a specific group or segment with the highest value. Positioning is your unique selling proposition for the target segment you have selected. 

## So, with the help of Excel, we imported 2,021 row data set (year=2020) and learned:
The "36-50" and "51-65" age groups are the biggest spenders at the food delivery platform, where the "36-50" age group spent 236,467, and the "51-65" age group spent 220,580.

The "high-income" group are the biggest spenders they spent a total of 655,186, followed by the "upper-middle" income group they have spent 348,070, making these two groups as potential target segments for the company.

The data suggests that in-store purchases are the favourite channel used by 11,737 customers, followed by website purchases made by 8,317 customers, then purchases made through a catalogue by 5,345 customers, and lastly purchasing by discounts by 4,709 customers.

<img src="images/pic1_marketing.jpg?raw=true"/>

<img src="images/pic2_marketing.jpg?raw=true"/>

You can find the same dataset used in this analysis in Kaggle, click here to access the link. It includes 2,021 rows and 44 different attributes. The Key attributes that I used in segmenting the data, are the total amount purchased by customers, customer income, customer age, and purchasing behaviour across different channels. 

Kindly note that there are other attributes available in the dataset that are not used in the analysis that can also be useful.

The analysis was done in Excel, using a nested IFS statement formula to segment the data by income and age, which is done by adding new columns for the "age group" and "income group" data. Then a pivot table and a bar chart was created using the total amount purchased column.

For the purchasing behaviour, I've created a pivot table including the demographic groups "age" and "income" and include four data columns related to purchasing behaviour. These are purchases made by the website, catalogue, in-store, and discounts. 

## A few groups clearly stood out in terms of spending:
Customers in the "high-income" bracket aged "36-50" spent a total of 236,467 at the delivery platform, making them the highest-spending group overall.

On the other end, customers aged "66 and above" in the "low-income" bracket spent only 2,776, the lowest amount among all groups.

The data suggests that the high-income group, especially those aged "36-50" and "51-65", are the most favourable target segments for the company’s future marketing positioning.

The upper-middle income group in the "51-65" age bracket also looks promising as a potential target, they have spent a total of 154,076.

<img src="images/pic3_marketing.jpg?raw=true"/>

In terms of customers buying habits, in-store purchases were the most common channel used by customers, with about 39% of all users (11,737 customers) choosing this method, followed by website purchases 27% (8,317 customers), then catalogue purchases 18% (5,345 customer), then buying from discounts 16% (4,709 customers).

<img src="images/pic2_marketing.jpg?raw=true"/>

4,265 customers in the "high-income" group bought most of their goods in store, followed by 3,849 customers in the "upper-middle" income bracket bought their products in store.

<img src="images/pic4_marketing.jpg?raw=true"/>

4,585 customers in the "36-50" age group bought their goods in store, the next potential age group segment is the "51-65", where 4,242 customers bought their products in store.

<img src="images/pic5_marketing.jpg?raw=true"/>

The "upper-middle" income group made the most purchases across all channels, but the highest sales amounts still came from the "high-income" and "36-50" age groups, who prefer in-store shopping over buying with discounts.

<img src="images/pic6_marketing.jpg?raw=true"/>

## Here is how to execute and nested IFS statement in Excel:
Go to the column you want to create groups for. Then, insert a new column to the right of the income column for example. Enter this formula:

=IFS(AND(Cell#>=1700,Cell#<=35400),"low",

 AND(Cell#>=35401,Cell#<=51400),"lower-middle",

 AND(Cell#>=51401,Cell#<=68200),"upper-middle",

 Cell#>=68201,"High",TRUE,"F")

(Note: Cell# refers to the first cell of the attribute you want to group in this case the income cell. For the income values don't insert commas in the thousands excel does not recognize commas in the formula).

## Recommendations: 
The High income and Upper-middle income groups in the "36-50" "51-65" age groups, is a potential target segment for the company's brand positioning strategy. What is interesting, is that both income groups can be reached by in-store, through a website, and by reading a catalogue. The company's positioning statement can be, "the no.1 delivery service provider with products tailored specifically for busy families". 

A practical takeaway from this project is that grouping customers by income, age, and buying behaviour in Excel using nested IFS formulas is a powerful way to segment a market. By setting up clear income brackets, you can quickly segment and analyse customer behaviour in large datasets, an approach that can be easily applied in other marketing projects.

