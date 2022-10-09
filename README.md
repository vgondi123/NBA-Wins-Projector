# NBA Wins Projector

## Description
What I set out to accomplish with this project was to be able to build a predictive model that could predict the number of games an NBA team will win. While many NBA predictive models predict how many wins a team will have based on in-season stats, I wanted my model to predict wins on a different basis. My model only uses statistics from seasons prior to the target season. This was done because the sole purpose of what I set out to do was to figure out which teams will be good or not before the season starts. To create the model, three methods of data science were used: web scraping, exploratory data analysis, and machine learning.

## Setup
I used Jupyter Notebook with Python as the language to complete this project.

## Part 1 - Web Scraping
To be able to create the dataset I wanted, I used the website https://www.basketball-reference.com/. This site comprises of a large amount of statistics of both basketball teams and players, dating back to the 1940s. My dataset uses statistics from 2012 and forward. The features I wanted to include in my dataset were the year of the season, team name, average age of the team, games played by the team in the season, total wins in the season, total losses in the season, win/loss % of the season, average experience of the team, coach's total experience, coach's career win/loss %, average career PER of the team, average career WS of the team. PER measures a player's per minute productivity. WS measures how many wins can be contributed to an individual player. In order to gather average experience of the team, coach's total experience, coach's total experience, coach's career W/L%, PER, and WS concurrent web scrapers were used. Concurrency was used because in order to gather these specific stats multiple links were required to be visited to gather one instance of a statistic. Using nested for loops caused execution time to be rather long. The use of concurrency improved the execution time of these web scrapers tremendously. After the web scraping process was finished, I cleaned up the dataset. 
<img width="1373" alt="Screen Shot 2022-10-02 at 10 47 52 PM" src="https://user-images.githubusercontent.com/91444902/193509110-c7a71bf2-1777-4127-bb4c-da2d36feeaac.png">
<img width="1371" alt="Screen Shot 2022-10-02 at 10 49 43 PM" src="https://user-images.githubusercontent.com/91444902/193509295-6cacaa56-555b-4553-9a2a-a8c924b652cd.png">
<img width="1366" alt="Screen Shot 2022-10-02 at 10 50 31 PM" src="https://user-images.githubusercontent.com/91444902/193509629-b88a61ab-bed8-434f-9621-5d5c2bf872ea.png">
<img width="1365" alt="Screen Shot 2022-10-02 at 10 51 51 PM" src="https://user-images.githubusercontent.com/91444902/193509702-9dd178bc-153a-4424-8794-cf238f2d9fc3.png">
<img width="1365" alt="Screen Shot 2022-10-02 at 10 55 10 PM" src="https://user-images.githubusercontent.com/91444902/193509907-0639fbc9-02af-4861-9d5e-cc8dc55d445f.png">

## Part 2 - Exploratory Data Analysis
The next part of the project involved exploratory data analysis in order to figure which variables would be used in the predictive model.
<img width="387" alt="Screen Shot 2022-10-02 at 11 08 50 PM" src="https://user-images.githubusercontent.com/91444902/193511423-1a9f50f3-034f-4b7f-a8f3-74a22f15cf6a.png">
<img width="411" alt="Screen Shot 2022-10-02 at 11 10 24 PM" src="https://user-images.githubusercontent.com/91444902/193511516-fb28850c-0cff-4f06-b373-b961ed206d23.png">
<img width="242" alt="Screen Shot 2022-10-02 at 11 11 49 PM" src="https://user-images.githubusercontent.com/91444902/193511664-c62c1232-8d2b-43f0-864a-563916fbaadd.png">
<img width="413" alt="Screen Shot 2022-10-02 at 11 12 13 PM" src="https://user-images.githubusercontent.com/91444902/193511779-bb5df726-3869-4acb-b25a-03fd7914b8f2.png">
<img width="378" alt="Screen Shot 2022-10-02 at 11 12 26 PM" src="https://user-images.githubusercontent.com/91444902/193511799-3cb34d52-e318-49d5-b10d-6f5301ed8547.png">

## Part 3 - Machine Learning

### Linear Regression Model
<img width="1361" alt="Screen Shot 2022-10-02 at 11 16 21 PM" src="https://user-images.githubusercontent.com/91444902/193512244-ba05020b-857c-4987-bf1b-3ddd9dc7d91b.png">
<img width="367" alt="Screen Shot 2022-10-02 at 11 17 13 PM" src="https://user-images.githubusercontent.com/91444902/193512361-fb51cac6-ce91-42c9-86af-695ba035b2b4.png">

### k-Nearest Neighbors Model
<img width="1355" alt="Screen Shot 2022-10-02 at 11 19 32 PM" src="https://user-images.githubusercontent.com/91444902/193512779-dea2ee3d-7489-442f-9889-96cd2533658b.png">
<img width="379" alt="Screen Shot 2022-10-02 at 11 19 58 PM" src="https://user-images.githubusercontent.com/91444902/193512794-bab86b70-957c-47d2-9123-b42a7721a3bf.png">
