## Effect of Health, Economics, Generosity, and Freedom of Choices to Happiness Index Around the World

<p style="text-align: center";> <b>Team Theta</b><br>Prasetyo Safira Putri
    <br>Minwoo Park</p>

------

#### 📌 General Idea 

Everyone wants to be happy, indeed. Even as a people we do not know exactly what makes us feel happy. There are factors that affect happiness which many studies and surveys have been conducted around the world. Those data are accessible as open data on Internet platforms. In order to recognize what makes us happy, we can properly compare the data related to the happiness index with several factors that could affect happiness. 

<br><br>

#### 📌 Datasets we used

We used the “world happiness  report” provided by Kaggle open data from 2017 ~ 2021 

2017 - 2019 https://www.kaggle.com/datasets/unsdsn/world-happiness

2020 https://worldhappiness.report/ed/2020/#appendices-and-data

2021 https://worldhappiness.report/ed/2021/#appendices-and-data

<br>There are several data such as Happiness, GDP, Family, Health, Freedom of choices, Trust (government corruption rate), Social support, and Generosity. In this project, we used 

+ Happiness
+ GDP
+ Health
+ Freedom of choices,
+ Generosity

as our main factors to compare. Because the family data is only available from 2017-2016 and 2016-2022 the family index changed into social support, so we don't want to compare different things. We also didn't use the corruption rate due it is not directly linked to individuals.

<br>

Those factor’s value came from : 

+ Freedom to make life choices is the national average of responses to the question “Are you satisfied or dissatisfied with your freedom to choose what you do with your life?”
+ Generosity is the residual of the regressing national average in response to the GWP question “Have you donated money to a charity in the past month?” on GDP per capita
+ Economics are from GDP per capita
+ Health is from Healthy Life Expectancy (HLE). Healthy life expectancies at birth are based on the data extracted from the World Health Organization’s (WHO).

<br><br>

#### 📌 Possible benefits for the users

We compared the index of happiness with the index of health, economics, generosity, and freedom for people to make choices and find out the factors that have the greatest influence on happiness among them. We also show the place where you can live with the most satisfaction of those among factors. 

<br><br>

#### 📌 What we made

##### Maps

We made 5 maps about happiness, GDP, health, Freedom, Generosity. There are the maps about each county's score for each factor. If the country's color is more clear and less bright, It means that the happiness ranking of that country is more high.

If you look world happiness map and look Austria for example, you can see that country's happiness score is about 7.2 and the ranking is 10th among 147 countries. 

Also you can zoom in and zoom out the map by click the map or scroll the mouse wheel up and down. If you put mouse cursor on the each degree of the diagram below, you can see which countries are in each degree. And the countries in the gray color are provided by the Anychart API, but not included in the open data set we use so we cannot access in that country. 

You can see the GDP map by click the button and move to another map. It is the map about GDP factor and same as the previous map, you can see each country's information. For example, Austria has about 10.9 GDP score and the ranking is 11th that is quite high. Like this way, you can also see the map of Health, Freedom, Generosity and you can return to the graph page. 

<br>

##### How we made it

At the first time to make a world map, I tried to use Leaflet API that we learned during our class. but after searching about many APIs about making world map, I thought that Anychart API is more suitable for making gradient map. So I used Anychart API in our project.

To give you a brief explanation of how we made the map, there are country codes that consists of two-letter for each country. If I add each country's code into the happiness data and connect these data with the map API that provided by Anychart, they show each country's happiness data in each region of the map based on the country code of each country.

<br>

##### Example

Gradient maps of world happiness index in every region![img](https://lh6.googleusercontent.com/9tdhnfLwEFQ01R6YZOCixnCEkJCsL1JzLLQ1V9b_K3iQmGx4M_7676F6KDfL7vEsTuVVZXGFmI8sukvDWxRCjcvgXw1j0SnI6y5mvV5ydvToDkY-VwJgA_CXWplRFm5k6AcOlF4XoG7aLa1WPx4JL9w)

<br><br>

##### Graphs

We made a graph of every sector (ex: economics) vs happiness index. We made a linear regression of it and compare the slope of it. The sector that has the highest slope must be the factor that has the greatest influence on happiness.

the graphs shows that the freedom of choices is the most significant factor that affects happiness followed by health, economics, and generosity. 

<br>

**Example** 

Comparison with Slope

![img](https://lh4.googleusercontent.com/TOFSB-QQrxk7LVmrScxUMsYS4Znb-UJKCIO5FMZI2sN4MvA8trA_-1qBgXMsV-6IhLokEML3Frjg4xvamHzzrWbBhJ9IYKEtlDCZbpR-3A-2wBezQLwZyWQ_I7c7FL7jzBQIk9XYADXU2ecNSdYocmc)

