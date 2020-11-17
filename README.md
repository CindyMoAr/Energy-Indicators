# Energy-Indicators
Data Cleaning Pandas

*Excel file Energy Indicators.xls, which contain a list of indicators of energy supply and renewable electricity production from the United Nations for the year 2013

##### Tasks:

1. Keep in mind that this is an Excel file, and not a comma separated values file. Also, make sure to exclude the footer and header information from the datafile. The first two columns are unneccessary, so you should get rid of them, and you should change the column labels so that the columns are:
['Country', 'Energy Supply', 'Energy Supply per Capita', '% Renewable']

2. Convert Energy Supply to gigajoules (there are 1,000,000 gigajoules in a petajoule). 

3. For all countries which have missing data (e.g. data with "...") make sure this is reflected as np.NaN values.

4. Rename the following list of countries (for use in later questions):

   "United States of America": "United States",
   "United Kingdom of Great Britain and Northern Ireland": "United Kingdom",
   "China, Hong Kong Special Administrative Region": "Hong Kong"```

5. There are also several countries with numbers and/or parenthesis in their name. Be sure to remove these, 

   e.g. Bolivia (Plurinational State of) should be 'Bolivia' 
       'Switzerland17' should be 'Switzerland'
       

*World_bank.csv is a csv containing countries GDP from 1960 to 2015 from [World Bank](http://data.worldbank.org/indicator/NY.GDP.MKTP.CD).

##### Tasks:
1. Load the GDP data. Make sure to skip the header.
2. Rename the following list of countries:
   "Korea, Rep.": "South Korea", 
   "Iran, Islamic Rep.": "Iran",
   "Hong Kong SAR, China": "Hong Kong"

*[Sciamgo Journal and Country Rank data for Energy Engineering and Power Technology](http://www.scimagojr.com/countryrank.php?category=2102) from the file `scimagojr-3.xlsx`,  ranks countries based on their journal contributions in the aforementioned area. 

##### Tasks:
1. Load de data. Call this DataFrame **ScimEn**.
2. Join the three datasets: GDP, Energy, and ScimEn into a new dataset (using the intersection of country names). Use only the last 10 years (2006-2015) of GDP data and only the    top 15 countries by Scimagojr 'Rank' (Rank 1 through 15). 

   The index of this DataFrame should be the name of the country, and the columns should be ['Rank', 'Documents', 'Citable documents', 'Citations', 'Self-citations',
       'Citations per document', 'H index', 'Energy Supply',
       'Energy Supply per Capita', '% Renewable', '2006', '2007', '2008',
       '2009', '2010', '2011', '2012', '2013', '2014', '2015'].

