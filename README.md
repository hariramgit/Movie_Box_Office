# Movie_Box_Office
The main goal of this project was to come up with a model to predict the international box office revenue of a movie based off a number of known data. 


# Project Description

## Data Set Information:


The main goal of this project was to come up with a model to predict the international box office revenue of a movie based off a number of known data. A model like this could be useful for production companies or studios to decide what kinds of movies to make, for distributors to estimate how much money to dedicate to marketing, or for cinemas to know more about the types of movies that make the most money.

The requirements for the project were to scrape HTML from a website using Beautiful Soup or Selenium, and then perform regression analysis on the data using Python packages from Scikit-learn or StatsModels.

In the end, the r-squared value for my model ended up being about .29, indicating that only 29% of the variance for international box office revenue was due to the features in my model.

---
### Deliverables
- `movies_scraping.ipynb`- scraping data from site, basic cleaning
- `top1000.pkl` - pickled dataframe after scraping
- `movies_regression.ipynb` - regularization, validation, regression analyses, feature engineering

---
### Data
Box Office Mojo: [Top 1000 movies by worldwide gross](https://www.boxofficemojo.com/chart/top_lifetime_gross/?area=XWW)

---
### Tools
Python packages: BeautifulSoup, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

---
### Variables

**Target variable**: International box office revenue

**Original features**: </br>
- year
- budget
- release month
- runtime
- ratings (yes or no): G, PG, PG-13, R
- genre (yes or no): action, adventure, animation, biography, comedy, crime, documentary, drama, family, fantasy, history, horror, music, musical, mystery, romance, sci-fi, sport, thriller, war, western

**Final features, pared down by Lasso regression**: </br>
- Positive correlation: 
  - year
  - budget
  - runtime
  - G rating
  - genres: adventure, animation, comedy </br>
- Negative correlation: 
  - release month
  - genres: action, biography, crime
  
  
  
  ### Task performed
- importing required models
- Uploading datasets
- performing EDA
- Removing and combining the data
- Feature extractions
- Model selection and implementing the best model
- Predicting and visualing



### steps we did in scraping:

- Importing required datasets
- 1st we are scraping data from the website by beautiful soup
- Cleaning and converting the data types
- Create a dictionary for the movie page details
- Scraping all movie details by separetly and stored
- Performig additional cleaning the data
- I save it to CSV to use in another notebook for my regression analysis.

### steps we did in regression analysis:

- Importing required datasets
- Importing our saved csv scrapped datasets file
- MultiLabelBinarizer to turn the genre column (of lists) into their individual columns
- performing EDA and converting variables to numeric variables by pd.dummies
- some regression experimentation the huge outliers
- Simple Validation
- Standard Linear Regression
- Polynomial Regression
- Ridge
- Eliminating Features with Lasso CV
- Droping sme columns and performing the models
- Performing Cross Validation
- scaling the datas EDA
- Examining Outliers
- Regularization after dropping more outliers
- Interpretation of Coefficients
- Residuals vs. Predictions
- RMSE
- LARS Path




### Analysis
#### Result analysis:


## Final LASSO path analysis image

![Final LARS path analysis image](https://github.com/hariramgit/Movie_Box_Office/blob/d0a4a14b80b4171e6f115363e4a8a6a56483ec22/OUTPUT%20IMAGE/lars%20path.png
)



## 🏗️ Built with
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)



## 👩‍💻 Libraries used



![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup-2C2D72?style=for-the-badge&logo=BeautifulSoup&logoColor=purple)
![Pandas](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=purple)
![Numpy](https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=yellow)

![Matplotlib](https://img.shields.io/badge/Matplotlib-F7931E.svg?style=for-the-badge&logo=Matplotlib&logoColor=orange) 
![seaborn](https://img.shields.io/badge/Seaborn-2C2D72?style=for-the-badge&logo=Seaborn&logoColor=blue)
![scikitLearn](https://img.shields.io/badge/scikitLearn-2C2D72?style=for-the-badge&logo=scikitLearn&logoColor=blue)



### Important models were used in this project:

- Encoding
- train_test_split
- MultiLabelBinarizer 
- metrics - mean_squared_error
- LinearRegression
- RIDGE,LASSO
- Polynomial Regression
- PolynomialFeatures
- Ordinary Least Squares class
- KFold




## Find the datasets here 

Box Office Mojo: [Top 1000 movies by worldwide gross](https://www.boxofficemojo.com/chart/top_lifetime_gross/?area=XWW)

Mine web sraped file:  https://github.com/hariramgit/Movie_Box_Office/blob/e290347f1f417c572c99903dbdcd4e17ac2216dd/top1000.pkl


## Organization
-  you may find the main Python Notebooks produced by the team members to realize the analysis, visualisations and predictive models.

SCRAPING FROM WEBSITE Repository --------(https://github.com/hariramgit/Movie_Box_Office/blob/e290347f1f417c572c99903dbdcd4e17ac2216dd/code/scraping.ipynb)

MOVIE BOX OFFICE ANALYSIS Repository ----------(https://github.com/hariramgit/Movie_Box_Office/blob/e290347f1f417c572c99903dbdcd4e17ac2216dd/code/movie%20box%20office%20revenue.ipynb)


 ## *Group project.* 
 
HARIRAM

MAHENDREN KUMAR


* [Email](mailto:hariramhdmp@gmail.com)



## 🤝 Support
Contributions, issues, and feature requests are welcome!
Give a STAR if you like this project! and FOLLOW do SUPPORT Friends...
 
- I hope you found the project useful and interesting. Feel free to contact me if you have any queries or suggestions...
