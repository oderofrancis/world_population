#  **WORLD POPULATION**

## Parse HUb software

World population CSV file was extracted using Parse software

ParseHub is a software tool that allows users to extract data from websites. It uses a visual interface to guide users through the process of selecting the data they want to extract, and then automatically scrapes the data from the website. ParseHub can handle websites that use dynamic content, such as web pages that load new data when the user scrolls down or clicks on a button. It can also scrape data from multiple pages on a website and handle complex navigation patterns.

check out this https://www.parsehub.com/

## API

An API, or Application Programming Interface, is a set of rules and protocols that allows different software applications to communicate with each other. In the context of Python, an API can be thought of as a set of functions and methods that allow a programmer to access and use the capabilities of a particular library or framework. For example, the Python standard library includes a wide variety of APIs that allow a programmer to perform tasks such as opening and reading files, working with data structures, and communicating over networks. Many third-party libraries and frameworks also provide their own APIs that can be used to perform specific tasks or access particular functionality. To use an API in Python, you will typically need to import the relevant library or module and then call the functions or methods provided by the API to perform the desired task.

```python

import requests
import json

r = requests.get("URL")
j=r.json()
print(j)

```

## Data scrapping using codes

Beautiful Soup is a Python library that is used for web scraping. It is used to extract data from HTML and XML files and can be used to easily extract information from websites. To use Beautiful Soup, you will first need to install it. This can be done using the pip package manager by running the following command:

`pip install beautifulsoup4`

Once Beautiful Soup is installed, you can use it to parse HTML and extract information from a website. Here is a simple example that demonstrates how to use Beautiful Soup to extract all the links from a web page:

```python
from bs4 import BeautifulSoup
import requests

# Make a GET request to the website
response = requests.get('http://www.example.com')

# Parse the HTML of the website
soup = BeautifulSoup(response.text, 'html.parser')

# Extract all the links from the page
links = soup.find_all('a')

# Print the links
for link in links:
    print(link.get('href'))
    
```
    
Beautiful Soup provides many other useful methods for parsing HTML and extracting information from a website. You can read more about it in the official documentation: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
