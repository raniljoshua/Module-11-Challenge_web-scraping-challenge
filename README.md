# Module-11-Challenge_web-scraping-challenge

Conducted a full web-scraping and data analysis, by extracting information via both automated browsing with Splinter and HTML parsing with Beautiful Soup, in order to produce the following deliverables:
* Deliverable 1: Scrape titles and preview text from Mars news articles.
* Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

Deliverable 1: Scrape titles and preview text from Mars news articles
----------------------------
* Used automated browsing to visit the Mars news siteLinks to an external site. Inspected the page to identify which elements to scrape.
* Created a Beautiful Soup object and used it to extract text elements from the website.
* Extracted the titles and preview text of the news articles that was scraped. Stored the scraping results in Python data structures as follows:
  * Stored each title-and-preview pair in a Python dictionary and, gave each dictionary two keys: title and preview.
  * Stored all the dictionaries in a Python list.
  * Printed the list.
 
Deliverable 2: Scrape and analyze Mars weather data, which exists in a table
----------------------------
* Used automated browsing to visit the Mars Temperature Data SiteLinks to an external site. Inspected the page to identify which elements to scrape.
* Created a Beautiful Soup object and used it to scrape the data in the HTML table.
* Assembled the scraped data into a Pandas DataFrame. Explanation of the column headings:
  * id: the identification number of a single transmission from the Curiosity rover
  * terrestrial_date: the date on Earth
  * sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
  * ls: the solar longitude
  * month: the Martian month
  * min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
  * pressure: The atmospheric pressure at Curiosity's location
* Examined the data types that are currently associated with each column. If necessary, casted (or converted) the data to the appropriate datetime, int, or float data types.
* Analyzed the dataset by using Pandas functions to answer the following questions:
  * How many months exist on Mars?
    * "There are 12 months on Mars."
  * How many Martian (and not Earth) days worth of data exist in the scraped dataset?
    * "There are 1867 Martian days' worth of data."
  * What are the coldest and the warmest months on Mars (at the location of Curiosity)?
    * "Month 3 is the coldest, month 8 is the hotest month on Mars."
  * Which months have the lowest and the highest atmospheric pressure on Mars?
    * "Month 6 has the lowest atmospheric pressure, and month 9 has the highest atmospheric pressure on Mars."
  * About how many terrestrial (Earth) days exist in a Martian year?
    * "The distance from peak to peak is roughly 1425-750, or 675 days. A year on Mars appears to be about 675 days from the plot. Internet search confirms that a Mars year is equivalent to 687 earth days."
* Exported the DataFrame to a CSV file.
