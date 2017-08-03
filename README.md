# Sport-Scraper

Class that allows variable scraping of sports data. Scrapes regular season or playoff data for NBA or NHL players (so far). Uses 2 positional arguments and 4 keyword arguments to switch between the types of data to scrape. 

After importing, call help() for more specifications on what values to pass into the arguments. 

### Dependencies

```
BeautifulSoup4, and Requests
```

### Sample Code

```
scrape=sport_scrape(start=1990,end=2015,league="NBA",season="Playoff",form="Advanced") 
# filepath argument not shown

scrape.scraper()
```

The above code scrapes Advanced NBA Playoff Player Data from the 1989-1990 season to the 2014-2015 season. The default setting is to save the csv files to the working directory but that can be changed by setting a different filepath to the filepath argument. When setting year values for start/end, always refer to the latest year; e.g. if you want end to be the 2014-2015 season, set it to 2015.

Initializing the class picks out the corrects lists required for scraping but does nothing else. Calling .scraper() will do the actual scraping. 


