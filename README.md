# Country Clustering with Python
## Background
The purpose of this notebook is to recreate a project which was initially written in `R` and completed by me, K.M.,and K.T. (if y'all ever come across this, you know who you are).  While feeling pretty comfortable with `R`, I want to practice using `Python` data analysis tools to get a better feel for them.  The dataset used is found on [Kaggle and was collected by HELP International](https://www.kaggle.com/rohan0301/unsupervised-learning-on-country-data).
## Data Description
We have 167 countries reflected by 9 different socio-economic/health features:

| Variable | Description | Type     |
| :-------------: | :---------- | :-----------: |
|`country`|Name of country|`chr`|
|`child_mort`|Death of children under 5 years of age per 1000 live births|`dbl`|
|`exports`|Exports of goods and services per capita.  Given as %age of GDP per capita.|`dbl`|
|`health`|Total health spending per capita.  Given as %age of GDP per capita.|`dbl`|
|`imports`|Imports of goods and services per capita.  Given as %age of the GDP per capita|`dbl`|
|`income`|Net income per person|`int`|
|`inflation`|The measurement of the annual growth rate of the Total GDP|`dbl`|
|`life_expec`|The average number of years a new born child would live if the current mortality patters are to remain the same|`dbl`|
|`total_fer`|The number of children that would be born to each woman if the current age-fertility rates remain the same|`dbl`|
|`gdpp`|The GDP per capita.  Calculated as the Total GDP divided by the total population|`int`|

We will perform some **principal component analysis**, **k-means clustering**, and **hierarchical clustering** using scikit-learn and matplotlib.

## Running the notebook
1. Create a virtual environment (skip this if you already have an environment or are using something else)
```{shell}
$ conda create -n data_analysis
```

2. Clone the repository
```shell
$ git clone https://github.com/392781/Country-Clustering-Analysis.git
```

3. Install the required libraries
```shell
$ conda install pip
$ pip install -r requirements.txt
```
or
```shell
$ conda install --file requirements.txt
```

4. Run jupyter note book and use!
```shell
$ jupyter notebook
```