# PythonWebScraper
This is my first foray into Python. I am currently coding in NodeJS and React. React is a Javascript framework. After some investigation into what is a good first off project to learn Python with it has been suggested to make a web scraper.

My IDE is Visual Studio Code, I will use Github for version control.

I will use the Beautiful Soup library to scrape the website. To install Beautiful Soup you will need to run pip install beautifulsoup4 this will install the most current version of Beautiful Soup.

We will need to install a parser that will be able to scrape broken and perfect HTML. To install this run pip install lxml

To install the HTML5 lib parser you will need to run. pip install html5lib
We will need to install a http library, to install this you will need to run pip install requests This will be used to download a http library.

Create a file called scraper.py in this file we will need to import our packages that have been installed. To import these packages in the file run:
from bs4 import BeautifulSoup
import requests

To import the website into BeautifulSoup you will need to use a get request to run that.
source = requests.get('https://medium.com/).text

To see the site indented and see which tags are associated with each other the beautiful soup package has a a prettier command. to see this when you run the script.
soup = BeautifulSoup(source, 'lxml')
article = soup.find('article')

To access a certain part of the website you will need to treat it like an attribute and add. match = soup.title.text You are accessing the title part of a site with this command. This will also just print out the text of that specific part of the site.

To find a certain div of the site you are scraping you can use the inspect element on a chrome browser.
print(soup.prettify)

WRITTEN BY

Jason Byron Beedle


