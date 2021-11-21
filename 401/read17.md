# Web Scrape
Web scraping is a technique to automatically access and extract large amounts of information from a website, which can save a huge amount of time and effort

## Inspecting the Website
The first thing that we need to do is to figure out where we can locate the links to the files we want to download inside the multiple levels of HTML tags

**libraries should installed**

- requests: to access the url of site
- urllib.request
- time
- from bs4: BeautifulSoup: access individual item from site


## Methods to prevent web scraping
The administrator of a website can use various measures to stop or slow a bot. 

- Blocking an IP address either manually or based on criteria such as geolocation and DNSRBL

- Disabling any web service API that the website's system might expose.
- Bots sometimes declare who they are (using user agent strings) and can be blocked on that basis using robots.txt; 'googlebot' is an example. 

- Bots can be blocked by monitoring excess traffic
- Bots can sometimes be blocked with tools to verify that it is a real person accessing the site, like a CAPTCHA. 

- Commercial anti-bot services

- Locating bots with a honeypot or other method to identify the IP addresses of automated crawlers.
- Because bots rely on consistency in the front-end code of a target website, adding small variations to the HTML/CSS surrounding important data and navigation elements would require more human involvement 
- Websites can declare if crawling is allowed or not in the robots.txt file and allow partial access

***resources***

[Web Scrape](https://towardsdatascience.com/how-to-web-scrape-with-python-in-4-minutes-bc49186a8460)

[wikipedia-Web_scraping](https://en.wikipedia.org/wiki/Web_scraping)