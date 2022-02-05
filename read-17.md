# Web Scraping

- A technique to automatically access and extract large amounts of info from a website
- Using the websites terms and conditions can tell you what the data can be used for
- Don't download to rapidly
- Using inspect we can view the HTML structure
- `<a>` hyperlinks allow us access to the data

## Code

- Imports:
    `import requests`
    `import urllib.request`
    `import time`
    `from bs4 import BeautifulSoup`
- URL:
    `url = 'http://'`
    `response = requests.get(url)`
- BeautifulSoup:
    `soup = BeautifulSoup(response.text,"html.parser")`
- Find `<a>` tags:
    `soup.findAll('a')`
- Isolate link:
    `one_a_tag = soup.findAll('a')[38]`
    `link = one_a_tag['href']`
- Download/Flagger:
    `download_url = 'url'`
    `time.sleep(1)`
- Downloading a whole set of data:
`line_count = 1`
`for one_a_tag in soup.findAll('a'):`
    `if line_count >= 36:`
        `link = one_a_tag['href']`
        `download_url = 'http://web.mta.info/developers/'+ link`
        `urllib.request.urlretrieve(download_url,'./'+link[link.find('/turnstile_')+1:])`
        `time.sleep(1)`
    `line_count +=1`

## Useful Links

- [How to Web Scrape with Python](https://towardsdatascience.com/how-to-web-scrape-with-python-in-4-minutes-bc49186a8460)
- [Web scraping](https://en.wikipedia.org/wiki/Web_scraping)
- [Scrape Websites Without Getting Blocked](https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/)
- [Track Amazon Prices](https://www.youtube.com/watch?v=Bg9r_yLk7VY)