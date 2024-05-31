Challenge 11

---

# Mars News Web Scraping and Weather Data Analysis

## Overview
In this project, we scrape data from two sources related to Mars: Mars news articles and Mars weather data. We use automated browsing with Splinter and HTML parsing with Beautiful Soup to extract the required information. Then, we organize, analyze, and visualize the data to gain insights into Mars.

## What You're Creating
This project consists of two main deliverables:
1. Scrape titles and preview text from Mars news articles.
2. Scrape and analyze Mars weather data from a table.


## Instructions

### Part 1: Scrape Titles and Preview Text from Mars News
1. Open the Jupyter Notebook named `part_1_mars_news.ipynb` in the starter code folder.
2. Use automated browsing to visit the [Mars news site](https://mars.nasa.gov/news/).
3. Inspect the page using Chrome DevTools to identify elements to scrape.
4. Create a Beautiful Soup object and use it to extract text elements from the website.
5. Extract the titles and preview text of the news articles.
6. Store the results in a Python list of dictionaries with keys `title` and `preview`. Example:
   ```python
   {'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm",
    'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."}
   ```
7. Print the list in your notebook.
8. (Optional) Export the scraped data to a JSON file.

### Part 2: Scrape and Analyze Mars Weather Data
1. Open the Jupyter Notebook named `part_2_mars_weather.ipynb` in the starter code folder.
2. Use automated browsing to visit the [Mars Temperature Data Site](https://static.bc-edx.com/data/web/mars_facts/temperature.html).
3. Inspect the page to identify elements to scrape.
4. Create a Beautiful Soup object and scrape the data in the HTML table.
5. Assemble the scraped data into a Pandas DataFrame with the following columns:
   - `id`: Identification number of a transmission from Curiosity rover
   - `terrestrial_date`: Date on Earth
   - `sol`: Number of elapsed sols (Martian days) since Curiosity landed
   - `ls`: Solar longitude
   - `month`: Martian month
   - `min_temp`: Minimum temperature (Celsius) of a Martian day (sol)
   - `pressure`: Atmospheric pressure at Curiosity's location
6. Examine and convert data types as necessary.
7. Analyze the dataset to answer the following questions:
   - How many months exist on Mars?
   - How many Martian days worth of data exist in the dataset?
   - What are the coldest and warmest months on Mars? Plot the average minimum daily temperature for each month as a bar chart.
   - Which months have the lowest and highest atmospheric pressure on Mars? Plot the average daily atmospheric pressure for each month as a bar chart.
   - Estimate the number of terrestrial days in a Martian year by plotting the daily minimum temperature.
8. Export the DataFrame to a CSV file.

## Installation
To run this project, ensure you have the following Python packages installed:
- BeautifulSoup
- Splinter
- Pandas
- Jupyter Notebook

You can install these packages using pip:
```sh
pip install beautifulsoup4 splinter pandas jupyter
```

## Usage
1. Open Jupyter Notebook.
2. Run `part_1_mars_news.ipynb` to scrape Mars news titles and previews.
3. Run `part_2_mars_weather.ipynb` to scrape and analyze Mars weather data.

## License
This project is licensed under the MIT License.

---


