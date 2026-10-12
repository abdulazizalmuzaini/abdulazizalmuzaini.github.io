# Major Projects in the Eastern Horn of Africa - 2022 
 
In the eastern Horn of Africa, the period from 2020 to 2022 experienced intense and recurrent cycles of flooding and droughts. During 2019/2020 there were extreme rains that caused devastating floods. Furthermore, La Niña climate patterns reached extreme levels not seen in the last 70 years, causing severe droughts during the 2020-2023 period. In addition, deforestation and land degradation have negatively impacted the region's ability to resist extreme weather events. The main sectors affected by the weather conditions include agriculture, water resources, and health.  

Climate-related hazards triggered economic shocks, while social factors such as deforestation, migration, urbanization, and indebtedness exacerbated the crisis. For example, in Kenya 205,000 people migrated to Garissa County because of the drought. In Ethiopia, Kenya, and Somalia, 30 million people faced food insecurity in 2020-2022.  Drought has reduced food supplies and driven hyperinflation, particularly in Ethiopia, where inflation reached 30-35%. Some countries adopted export bans to secure their own food supplies, restricting access for nations dependent on food imports. [Click this link to read more about the Horn of Africa floods and drought, 2020-2023 - Forensic analysis](https://www.undrr.org/resource/horn-africa-floods-and-drought-2020-2023-forensic-analysis). 

The main aim of this article is to analyze the World Bank's International Development Association (IDA) dataset using SQL. The dataset is a snapshot of the November 2022 period made up of 9,998 rows. SQL query statements were performed using the online (CSVfiddle.io) platform. Specific research questions include: What was the total principal amount extended to Ethiopia, Kenya, and Somalia? What are the major IDA-funded projects in the eastern Horn of Africa? How much does each country owe the IDA? How much of the loans have been paid back to the IDA? How much has each country utilized the loans? How much of the loan is available for draw down for each country? 

<img src="images/pic1_worldbank.png?raw=true"/>

The total loan principal amount extended by the IDA to Ethiopia is US$ 29.1 billion, followed by US$18.4 billion for Kenya, and US$ 2.6 billion for Somalia. Through SQL, the data is filtered by country, and what is interesting is that the IN-clause acts similarly to the OR clause by combining several countries as multiple conditions. 

<img src="images/pic2_worldbank.png?raw=true"/>

<img src="images/pic3_worldbank.png?raw=true"/>

Total Due to IDA represents the outstanding balance at the end of the reporting period. It is what each country in the eastern Horn of Africa must pay back to the IDA. By splitting each country as its own category, the total due to IDA amounts for Ethiopia in 2022 was US$ 10.7 billion, Kenya US$ 10.1 billion, and Somalia US$ 104.7 million.  

<img src="images/pic4_worldbank.png?raw=true"/>

<img src="images/pic5_worldbank.png?raw=true"/>

Given the massive scale of loans extended to the Horn of Africa countries across numerous initiatives, this article focuses on three major projects. 

 In Kenya, the Inclusive Growth and Fiscal Development Policy Operation (DPO) was financed at US$ 750 million. The purpose of the project was to support Kenya's economic recovery following the COVID-19 pandemic and severe droughts. Additionally, the project aimed to provide social safety nets for disadvantaged households and expand digital financial inclusion for small and medium-sized enterprises. The project also aims to fund policy reforms including fiscal transparency, public procurement, public financial management, and fighting corruption. [Click here to watch the video about the project](https://www.worldbank.org/en/news/video/2022/03/16/kenya-receives-a-750-million-boost-to-support-economic-transformation-post-pandemic). 

In Ethiopia, the Growth and Competitiveness Project was funded by World Bank's IDA with a total amount of $US 600 million. The government aims to increase public investment in the agriculture and service sectors. However, Ethiopia has achieved only modest structural economic transformation and private sector development. The new leadership announced decisions to expand the role of the private sector, reform state-owned Enterprises, and enhance fiscal sustainability. [Click here to read more about this project](https://documents.worldbank.org/en/publication/documents-reports/documentdetail/446071551898567481#:~:text=De%20Facto%20Governments%2C%20Democratic%20Government%2C%20Economics%20and,Version%20Type.%20Final.%20*%20Product%20Line.%20IBRD%2FIDA.). 

In Somalia, one of the major IDA-funded projects was the Reengagement and Reform Development Policy Financing (DPF). The objective of this DPF is to normalize relations between Somalia and the World Bank Group, as well as make policy reforms such as improving fiscal management, enhancing private sector growth, building human capital, and strengthening climate resilience. The total loan amount was US$420 million subdivided into two tranches. The first tranche of US$ 375 million was designated to restructure Somalia's overdue debt, while the second tranche of US$ 45 million supported budget cash-flow needs. [Click here to access more information about this project](https://documents.worldbank.org/pt/publication/documents-reports/documentdetail/691651583636465400). The SQL Query used to find the top projects: 

<img src="images/pic6_worldbank.png?raw=true"/>

## Ethiopia:

<img src="images/pic7_worldbank.png?raw=true"/>

## Somalia:

<img src="images/pic8_worldbank.png?raw=true"/>

## Kenya:

<img src="images/pic9_worldbank.png?raw=true"/>

The total amounts repaid to the World Bank's IDA for each country in the eastern Horn of Africa, ordered from highest to lowest, show that Ethiopia has repaid the largest amount at US$ 3.9 billion. Kenya has repaid US$ 2.3 billion, and Somalia has repaid the lowest amount at US$ 308.87 million (noting that Somalia also borrowed the smallest loan amount from the IDA).

<img src="images/pic10_worldbank.png?raw=true"/>

<img src="images/pic11_worldbank.png?raw=true"/>

The total disbursed amount represents the total funds each country has withdrawn from its original loan allocation. Ethiopia has disbursed US$ 2.14 billion from its original loan, while Kenya and Somalia have disbursed US$ 1.32 billion and US$ 1.34 billion, respectively.  

<img src="images/pic12_worldbank.png?raw=true"/>

What portion of the undisbursed amount has been cancelled, and what funds remain available for each country to draw down?  In Kenya, out of a total undisbursed loan amount of US$ 3.4 billion, US$1.5 billion has been cancelled leaving a remaining balance of US$1.89 billion available for drawdown by the Kenyan government. In Ethiopia, the total undisbursed amount is US$5.9 billion, with US$1.3 billion cancelled, leaving US$4.6 billion available for drawdown. Finally, Somalia has total undisbursed amount of US$1.1 billion, of which US$ 162.1 million has been cancelled, leaving US$ 913.1 million available for the Somali government to drawdown. 

<img src="images/pic13_worldbank.png?raw=true"/>

<img src="images/pic14_worldbank.png?raw=true"/>

<img src="images/pic15_worldbank.png?raw=true"/>

<img src="images/pic16_worldbank.png?raw=true"/>

<img src="images/pic17_worldbank.png?raw=true"/>







