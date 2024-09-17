# Web-Scraping-Challenge
UCI Data Analyst Module 11 - Web Scraping Challenge

This module I created 2 Jupyter notebooks that scraped html data about Mars. The first Jupyter notebook inspected news articles and pulled the title and corresponding previews of the titles. In the second Jupyter notebook I scraped data from a table and used that table to perform calculations and analysis. 

## Jupyter Notebook 1
I used automated browsing to visit the Mars news site and inspected the page to identify which elements to scrape.

I created a Beautiful Soup object and used it to extract text elements from the website.

I extracted the titles and preview text of the news articles I scraped and stored the results in Python data structures as follows:

Each title-and-preview pair was stored in a Python dictionary, with each dictionary containing two keys: title and preview.
All the dictionaries were stored in a Python list.
I printed the list in my notebook.

Additionally, I stored the scraped data in a file for easier sharing. I exported the scraped data to a JSON file.

## Jupyter Notebook 2
I used automated browsing to visit the Mars Temperature Data site at https://static.bc-edx.com/data/web/mars_facts/temperature.html and inspected the page to identify which elements to scrape.

I created a Beautiful Soup object and used it to scrape the data from the HTML table. I then assembled the scraped data into a Pandas DataFrame with columns having the same headings as those on the website:

- **id**: The identification number of a single transmission from the Curiosity rover
- **terrestrial_date**: The date on Earth
- **sol**: The number of elapsed sols (Martian days) since Curiosity landed on Mars
- **ls**: The solar longitude
- **month**: The Martian month
- **min_temp**: The minimum temperature, in Celsius, of a single Martian day (sol)
- **pressure**: The atmospheric pressure at Curiosity's location

I examined the data types for each column and, if necessary, converted the data to the appropriate datetime, integer, or float types.

I analyzed the dataset using Pandas functions to answer the following questions:

1. **How many months exist on Mars?**
2. **How many Martian days worth of data exist in the scraped dataset?**
3. **What are the coldest and warmest months on Mars at the location of Curiosity?**  
   To answer this question, I calculated the average minimum daily temperature for all of the months and plotted the results as a bar chart.
4. **Which months have the lowest and highest atmospheric pressure on Mars?**  
   To answer this, I calculated the average daily atmospheric pressure of all the months and plotted the results as a bar chart.
5. **About how many terrestrial days exist in a Martian year?**  
   I estimated this by considering how many days elapse on Earth in the time that Mars circles the Sun once and visually estimated the result by plotting the daily minimum temperature of each observation.
   
Finally, I exported the DataFrame to a CSV file.

Worked with Brendan and Chris.

Used chatGPT to debug code.
