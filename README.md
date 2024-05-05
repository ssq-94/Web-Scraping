# Web-Scraping (Client Project)

# About the Project
The goal of this project is to scrape a watch brand's website to gather a set of data points about every watch. 
![image](https://github.com/ssq-94/Web-Scraping/assets/78969075/0db07d86-f334-43d6-af2c-c6d83546e241)

The project is divided into three major stages:

# Stage 1
- Data collection via web scraping.
- Data analysis - create a summary report in Python notebook.

# Stage 2 
- Data cleaning

# Stage 3 
- Pipeline automation using Airflow and Docker.

# Stage 1 Project Steps
## Step 1: Installations

Before starting the scraping process, you'll need to install the following dependencies:

- `selenium`- Python library for web automation and controlling web browsers programmatically.
- `webdriver`-  Google Chrome browser driver.
- `BeautifulSoup`- Library for parsing HTML and XML documents and extracting data from web pages.
- `requests`- Library used for making HTTP requests to retrieve web pages or resources.

## Step 2: Install WebDriver

1. Set the `chromedriver_path` variable to the path of  the ChromeDriver executable on your device.
2. Use the options variable is used to set options for Chrome, such as running it in headless mode.
3. Create a `webdriver.Chrome()` creates a Chrome WebDriver instance using the ChromeDriver executable.
4. Use `driver.get()` method opens the target website.
5. Add a delay of 5 seconds `time.sleep(5)` to allow the page to load.
6. Scroll down the page using `driver.execute_script("window.scrollTo(0, document.body.scrollHeight) ;")`.
7. Add another 5-second delay to allow the page to load more items.
8. Compare the new height of the page with the previous height to check if more items were loaded. If the heights are the same, it means there are no more items to load, and the loop breaks.
9. Repeat the process until all items on the page have been loaded.

## Step 3: Extracting Watch Data and Creating DataFrame

In this step, extract the relevant watch data from the website and create a DataFrame to store the information.

# Step 4: Data Analysis and Visualization

Perform data analysis and visualization on the selected columns using various charts. The charts include:
- Bar chart showing the distribution of dial colors.
- Pie chart showing the distribution of water resistance.
- Bar chart showing the distribution of case shapes.
- Bar chart showing the distribution of movement by brand.
