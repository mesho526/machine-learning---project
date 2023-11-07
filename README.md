# How to predict salary of an employee based on years of experience?
                      Mekibeb Yicheneku

  Predicting salary based on an individual's years of experience is a fundamental challenge in the field of machine learning and data science. In this project, our goal is to uncover the relationship between an employee's accumulated years of professional experience and their corresponding salary. Much like the quest to understand what drives success in various domains, we aim to unveil patterns and connections that illuminate how an individual's income evolves over the course of their career. By developing a regression model that utilizes historical salary and experience data, our project seeks to provide valuable insights into the question: What are the key factors that influence an individual's salary progression throughout their professional journey?
      In the dynamic world of workforce management and human resources, understanding the determinants of an individual's salary progression over the course of their career is of paramount importance. As careers unfold, many factors come into play, shaping an individual's income trajectory. Just as the performance of a basketball player can be evaluated by their average points per game, we seek to unveil the underlying dynamics that govern salary evolution. Our project, "Predicting Salary with Years of Experience," delves into this intriguing puzzle.
				

                                         INTRODUCTION
The easiest way to evaluate a salary of one’s employees  is to see how many year of experience he/she have. Welcome to 'Predicting Employee Salary from Years of Experience.' In the realm of workforce management and compensation analysis, the connection between an employee's salary and their accumulated years of professional experience is a pivotal focus. my project embarks on a data-driven journey to uncover the essential link between these two crucial elements. Much like evaluating an individual's career progression, my goal is to develop a robust predictive model that accurately estimates an employee's salary, with years of professional experience as the central factor. By accounting for additional variables such as education, industry, location, and potential bonuses, I aim to reveal the intricate interplay of these factors in shaping salary evolution. The insights derived from this endeavor have the potential to enhance compensation strategies and inform career planning, benefitting both organizations and individuals in the realm of workforce management and human resources.

				                  DATA COLLECTION
For my data collection process, I sourced relevant datasets from the online platform Kaggle, a reputable hub for various datasets and data science resources. The dataset we obtained comprises two crucial columns: the first column records years of professional experience, while the second column documents the corresponding salary information. This dataset serves as the foundational source for our project, providing us with real-world data to analyze and build our predictive model. The utilization of Kaggle as our data source ensures the credibility and reliability of the information, enabling us to delve into the intricate relationship between years of experience and employee salaries. Below are the first 4 rows of this dataset
              

To better understand this dataset, I can also visualize it by constructing a scatter plot , since it has only two properties to plot (year of experience and salary).


 
From this dataset, we can see that there might exist some relationship between years of experience and the salary, although the variation is relatively high. Next, I am going 
to build linear regression models over this dataset and analyze this data.
				
                       SIMPLE LINEAR REGRESSION
Simple Linear Regression (or SLR) is the simplest model in machine learning. It models the linear relationship between the independent and dependent variables.

In this project, there is one independent or input variable which represents the years of exprience data and is denoted by X. Similarly, there is one dependent or output variable which represents the salary data and is denoted by y. We want to build a linear relationship between these variables. This linear relationship can be modeled by mathematical equation of the form:-
			Y = β0   + β1*X    -------------   (1)
In this equation, X and Y are called independent and dependent variables respectively, β1 is the coefficient for independent variable and β0 is the constant term. β0 and β1 are called parameters of the model. For simplicity, we can compare the above equation with the basic line equation of the form:-
    			y = ax + b       ----------------- (2)
We can see that
Slope of the line is given by, a = β1, and
Intercept of the line by b = β0.
In this Simple Linear Regression model, we want to fit a line which estimates the linear relationship between X and Y. So, the question of fitting reduces to estimating the parameters of the model β0 and β1.
                                    
                                    EXPLORATORY DATA ANALYSIS
First, I import the dataset into the dataframe with the standard read_csv () function of pandas library and assign it to the salary_data variable. Then, I conducted exploratory data analysis to get a feel for the data. I checked the dimensions of dataframe with the shape attribute of the dataframe. I viewed the top 4 rows of the dataframe with the pandas head () method. I viewed the dataframe summary with the pandas info () method and descriptive statistics with the describe () method.
 
