# Mobile_Price_Classification_EDA_and_Machine_Learning
This notebook aims to Exploratory Data Analyst and build Machine Learning to classified the price of mobile phone

### About Dataset
The Dataset that I use was **Mobile Price Classification**. The dataset contains with 21 features with some categorical and numerical features. The target from this dataset is 'prica_range' which consists of 0(low cost), 1(medium cost), 2(high cost) and 3(very high cost).

### Background
Mobile is one of the most selling and purchasing device. Almost all peoples use it communicate, social media or another tasks. Every day new mobiles with new version and more features are launched. The number of users has already reached 3 billion, and this figure is only expected to climb over the next few years.

### Problem
In order able to fight with another companies, price is one of important things to deal before launch to market. Many features are important to be considered to estimates the price. So, its important to know the relation between the features and selling price to able compete in market.

### Goal
The main goals are:
1. Perform **Exploratory Data Analyst** between Features and Target to know the relation
2. Building **Machine Learning** to classify the price of mobile phone using some algorithms

### Result
`1. Exploratory Data Analyst`\
Here are some insight that I got from this EDA:
- Battery_power has **positive correlation** with price_range. The **more quality** of the battery_power will **increase** the price_range
- Whether or not bluetooth **does not really affect** the price
- clock_speed has **negative correlation** with price_range. The **smaller the speed** of execute intructions would **increase the price_range**
- Mobile phone with dual_sim also could be sell in all price_range. but it would be even better if we sell it at the **very high cost** for more revenue
- Mobile phone with **good Front Camera** (11-19 MP)  has higher estimates price_range
- Mobile phone with four_g also could be sell in all price_range. But it would be even better if we sell it at the **very high cost** for more revenue
- Mobile phone that **light** should be sell in **very high cost** while Mobile phone that **weight** could be sell in all price_range **except very high cost**
- Mostly mobile phone selled with **4 n_cores**. The price_range for 4 n_cores should be sell in **medium or high cost**
- ram has **positif correlation** with price_range. The higher ram, the higher price_range of mobile phone 
- The longest average of talk_time for **high battery** is around 11.50 hour with Very high price_range
- it is advisable to sell mobile phone with three_g because it could be sell in any price_range

`2. Machine Learning`\
I used some algorithms to classify the price of mobile phone. Here is the evaluation matrix:

| Model | Accuracy|
| ------- | -------- |
| SVC  | 0.915 |
| SVC Tuned | 0.965 |
| KNN  | 0.6025 |
| KNN Tuned | 0.8175 |
| Random Forest | 0.9025 | 
| Random Forest Tuned | 0.92|

**From some algorithms Machine Learning that I had tried, it turn out that SVC after Tuned has the highest Accuracy aroung 96.5%**
