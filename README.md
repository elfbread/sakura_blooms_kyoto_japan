# Sakura Season in Kyoto, Japan
 
Python and Tableau project for completion of the Code Louisville Data Analysis II course in Summer 2022.

Data Source: [Osaka Prefecture University](http://atmenv.envi.osakafu-u.ac.jp/aono/kyophenotemp4/) (both datasets available here)

This project includes data of peak cherry blossom bloom date in Kyoto, Japan back to the year 853. It also includes a dataset with average yearly temperature in Kyoto. The project does the following: imports the two CSV files from Google Sheets (to avoid broken file paths between Windows and MacOS); utilizes a left join to combine the two datasets on the shared field 'Year'; checks for and removes missing values; converts all columns from Celsius to Fahrenheit; generates quartiles; creates a new column assigning a category of 'Low', 'Medium', or 'High' based on the average temperature; and then exports the final table to .xlsx for ease of import into Tableau. 

After the data cleaning and export, the dataset is imported into Tableau Public. Two visualizations were created: a histogram showing the average dates of peak blooms from the time period and a scatterplot showing the relationship between average yearly temperature and peak bloom date. The final dashboard is available at [Sakura Blooms in Kyoto Dashboard](https://public.tableau.com/views/SakuraBloomsinKyotoProject/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link).

## Start-up instructions

Before starting, you need to download/install the following extensions in VS Code for Jupyter Notebook:

![Juypter Notebook](https://github.com/elfbread/pyAirports/blob/main/extension.png)

Clone the repo to your computer. 

Package requirements are listed in the requirements.txt file. Install the libraries in the requirements.txt file using the following command:

`pip install -r requirements.txt`

Packages used in this project include:

- numpy 
- pandas

Create and activate your virtual environment utilizing Command Prompt (more information available here: [venv set up and activation](https://www.freecodecamp.org/news/how-to-setup-virtual-environments-in-python/). Be sure to cd into your correct directory prior to setting up and activating your venv!

To create venv:

`python -m venv env`

To activate venv:

`env/Scripts/activate.bat`
 
Navigate to the folder and open main.ipynb with VS Code. Be sure to update the kernel in the upper right of VS Code (as shown in the screenshot below).The file imports uses public CSVs saved in my Google Sheets account, a work around for users utilizing different operating systems (not having to adjust the import statement/file path).

# Let's talk project requirements:

Features used:

****** NOTE: I have changed my project since submitting my project brief in mid-June 2022 ******

1. __Loading data.__ Two CSVs are loaded into Python (bloom dates dataset and average temperature dataset).
2. __Clean data, merge in pandas, and calculate a new value.__ Datasets were cleaned (missing values dropped, columns dropped), a left merge using pandas was implemented using the shared field "Year", and a new value was calculated (category assignment based on temperature: "Low", "Medium", "High").
3. __Tableau Dashboard was created.__ [Sakura Blooms in Kyoto Dashboard](https://public.tableau.com/views/SakuraBloomsinKyotoProject/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link).
4. __Virtual environment with instructions.__ A virtual environment was utilized and instructions on how to utilize it are provided in this README. A requirements.txt file is also included to install necessary packages and dependencies.
5. __Annotations in Jupyter Notebook.__ The main.ipynb file includes annotations on the purpose of the code blocks.
6. __Detailed README file with formatting.__ This README has been formatted using GitHub markup. 

