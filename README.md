# Web Scraping Challenge

![image](https://github.com/AnaTipps/web-scraping-challenge/assets/131827518/4b7f74e2-e818-4f8d-be51-8b6fd30ded55)


## Background
Now we are ready to take on a full web-scraping and data analysis project. For this assigment I've identifyed HTML elements on a page, their id and class attributes, and use this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup. I’ve also learned to scrape various types of information. These include HTML tables and recurring elements, like multiple news articles on a webpage.

#### This assignment consists of two technical products. That I submited in the two following deliverables:

Deliverable 1: Scrape titles and preview text from Mars news articles.

Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

## Part 1: Scrape Titles and Preview Text from Mars News

On the Jupyter Notebook  named part_1_mars_news.ipynb. I used automated browsing to visit the Mars news site. Inspect the page to identify which elements to scrape.

I Created a Beautiful Soup object and use it to extract the titles and preview text of the news articles that I scraped and stored the scraping results in a Python dictionary and, give each dictionary two keys: title and preview. An example is the following:

{'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm", 
 'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."}
Store all the dictionaries in a Python list.


## Part 2: Scrape and Analyze Mars Weather Data

On the Jupyter Notebook named part_2_mars_weather.ipynb. I used automated browsing to visit the Mars Temperature Data Site (https://static.bc-edx.com/data/web/mars_facts/temperature.html.)  and  inspected the page to identify which elements to scrape.
I then created a Beautiful Soup object and use it to scrape the data in the HTML table to then assemble the scraped data into a Pandas DataFrame. 

id: the identification number of a single transmission from the Curiosity rover
terrestrial_date: the date on Earth
sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
ls: the solar longitude
month: the Martian month
min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
pressure: The atmospheric pressure at Curiosity's location

I analyzed the dataset by using Pandas functions to answer the following questions:

How many months exist on Mars?

How many Martian (and not Earth) days worth of data exist in the scraped dataset?

What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:

Find the average minimum daily temperature for all of the months.

Plot the results as a bar chart.

Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:

Find the average daily atmospheric pressure of all the months.

Plot the results as a bar chart.

About how many terrestrial (Earth) days exist in a Martian year? To answer this question:

Consider how many days elapse on Earth in the time that Mars circles the Sun once.

Visually estimate the result by plotting the daily minimum temperature.


### And finaly I exported the DataFrames to  CSV files.
