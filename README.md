# Sakura Season in Kyoto, Japan
 
Python and Tableau project for completion of the Code Louisville Data Analysis II course in Summer 2022.

Data Source: [Osaka Prefecture University] (http://atmenv.envi.osakafu-u.ac.jp/aono/kyophenotemp4/) (both datasets available here)

This project includes data of peak cherry blossom bloom date in Kyoto, Japan back to the year 853. It also includes a dataset with average yearly temperature in Kyoto. The project does the following: imports the two CSV files from Google Sheets (to avoid broken file paths between Windows and MacOS); utilizes a left join to combine the two datasets on the shared field 'Year'; checks for and removes missing values; converts all columns from Celsius to Fahrenheit; generates quartiles; creates a new column assigning a category of 'Low', 'Medium', or 'High' based on the average temperature; and then exports the final table to .xlsx for ease of import into Tableau. 

After the data cleaning and export, the dataset is imported into Tableau Public. Two visualizations were created: a histogram showing the average dates of peak blooms from the time period and a scatterplot showing the relationship between average yearly temperature and peak bloom date. 

## Start-up instructions

Before starting, you need to download/install the following extensions in VS Code for Jupyter Notebook:

[Juypter Notebook] (https://github.com/elfbread/pyAirports/blob/main/extension.png)
