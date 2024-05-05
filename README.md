# Web-Scraping (Client Project)

# About the Project
Our goal is to scrape a watch brand’s website to get a set of data points about every watch. 

![image](https://github.com/ssq-94/Web-Scraping/assets/78969075/25ec0299-f525-4c68-be38-c6f35ac4a221)


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
- `selenium`- python library
- `webdriver`- for Google Chrome browser
  
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
