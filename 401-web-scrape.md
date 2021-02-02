# Web Scraping

> web scraping in a technique to access and extract large amounts of info wrom a wbsite

### important caveats
- read through term of website top see hwo you can legally use the data
- make sure you are not downloading too rapidy could crash the site

> firt you must inspect the web page


### libraries needed
- `import requests`
- `import urllib.request`
- `import time`
- `import bs4 import BeautifulSoup`

### set url to site and access with request lib
- `url = "siteurlhere"`
- `response = requests.get(url)`

> 200 status message means it was sucessfull

### parse data with BeautifulSoup
- `soup = BeautifulSoup(response.text,"html.parser")`

### use find all to find A tags
- `soup.findAll('a')`


### link extraction
- `one-a-tag = soup.findAll('a')[38]`
- `link = one-a-tag['href']`

- `download_url = 'http://web.mta.info/developers/'+ link
urllib.request.urlretrieve(download_url,'./'+link[link.find('/turnstile_')+1:])`

## preventing spamming
 - `time.sleep(1)`