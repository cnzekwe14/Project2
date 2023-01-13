Project: 

    1. In this project we're extracting, transforming and loading Olympic medal data spanning the years 1896 to 2021. Additionally, we're executing the extract, transform and load process for data from the Human Development Index (HDI) for follow-on analysis on the potential relationships between Olympic performance and HDI rankings. 

Extraction: 

    1. The 'Olympics_medals_country_wise.csv' was extracted from Kaggle. This csv contains 17 columns and 156 countries worth of data. 

    2. The 'Human Development Index - Full.csv' was extracted from Kaggle. This csv contains 880 columns and 195 countries worth of data. 

Transformation: 

    1. The aforementioned olympic and HDI data were read into Jupyter Notebook and named 'Olympic Country Data.ipynb'. Initial observations were performed by viewing the data in Pandas dataframes. 

    2. A total of three distinct steps were performed to clean our data, including the removal of unwanted characters for standardizing the data across both data sets, as well as renaming columns, and converting data types. 

    3. We subsequently merged our datasets using the shared country column, resulting in a 126 row, by 896 column merged dataframe. This merged dataframe was converted into the 'Olympic_Country_Data.csv' dataset. 

Loading: 

    1. The 'Olympic_Country_Data.csv' dataset was imported and converted into a MongoDB database named 'Olympic_Country_Data' with a collection named 'all_olympics'. These steps can be viewed in the 'Mogodb_Olympics.ipynb' file.    