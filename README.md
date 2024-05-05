# Web-Scraping (Client Project)

# About the Project
Our goal is to scrape a watch brand’s website to get a set of data points about every watch. 

![image](https://github.com/ssq-94/Web-Scraping/assets/78969075/0db07d86-f334-43d6-af2c-c6d83546e241)


We have 3 major tasks broken into different stages:

# Stage 1
- Data collection via web scraping.
- Data analysis - create a summary report in Python notebook.

# Stage 2 
- Data cleaning

# Stage 3 
- Pipeline automation using Airflow and Docker.


# Stage 1 Project Steps

## Step 1: Installations
To start scraping, you'll need to install the items below.
- `selenium`- Python library
- `webdriver`-  Google Chrome browser
- `BeautifulSoup`- Extracting data from web pages.
- `requests`- Used for making HTTP requests to retrieve web pages or resources.
  
#### More Info

- `selenium:` Used for web automation and controlling web browsers programmatically.
- `webdriver:` Provides a way to start and control a web browser using Python.
- `By:` Provides mechanisms for locating elements on a web page.
- `WebDriverWait and expected_conditions:` Used for waiting until certain conditions are met before proceeding with code execution.
- `Keys:` Provides special keys (e.g., Enter, Shift) for simulating keyboard actions.
- `BeautifulSoup:` Used for parsing HTML and XML documents and extracting data from web pages.
- `time:` Provides time-related functions, such as adding delays in code execution.
- `requests:` Used for making HTTP requests to retrieve web pages or resources.
- `csv:` Provides functionality for reading and writing CSV files.
- `pandas:` Widely used for data manipulation and analysis, with DataFrames for working with tabular data.
- `pd.set_option('display.max_columns', None):` Sets an option in pandas to display all columns when printing DataFrames.
- `re:` Provides support for regular expressions, used for pattern matching and text manipulation.

## Step 2: Install WebDriver

1. The `chromedriver_path` variable specifies the path to the ChromeDriver executable on your device.
2. The options variable is used to set options for Chrome, such as running it in headless mode.
3. The `webdriver.Chrome()` creates a Chrome WebDriver instance using the ChromeDriver executable.
4. The `driver.get()` method opens the target website
5. The `time.sleep(5)` waits for 5 seconds to allow the page to load.
6. The code then scrolls down the page using `driver.execute_script("window.scrollTo(0, document.body.scrollHeight) ;")`.
7. It waits for 5 seconds again to allow the page to load more items.
8. The code calculates the new height of the page and compares it with the previous height to check if more items were loaded. If the heights are the same, it means there are no more items to load, and the loop breaks.
9. The process continues until all items on the page have been loaded.

## Step 3: Extracting Watch Data and Creating DataFrame


# Step 4: Data Analysis and Visualization
In this Step, the selected columns are analyzed and visualized using various charts.

- The first chart is a bar chart showing the distribution of dial colors.
- The second chart is a pie chart showing the distribution of water resistance.
- The third chart is a bar chart showing the distribution of case shapes.
- The fourth chart is a bar chart showing the distribution of movement by brand.
