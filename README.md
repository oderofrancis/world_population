# world_population

## Parse HUb software

World population CSV file was extracted using Parse software

## API

An API, or Application Programming Interface, is a set of rules and protocols that defines how two pieces of software should interact with each other. It's essentially a way for different software programs to communicate with each other and share data and functionality.

Basically, an API specifies how software components should interact.
Additionally, APIs are used when programming graphical user interface (GUI)
components.

A good API makes it easier to develop a program by providing all the
building blocks. A programmer then puts the blocks together.

## Data scrapping using codes

Beautiful Soup is a Python library that is used for web scraping. It is used to extract data from HTML and XML files and can be used to easily extract information from websites. To use Beautiful Soup, you will first need to install it. This can be done using the pip package manager by running the following command:

`pip install beautifulsoup4`

Once Beautiful Soup is installed, you can use it to parse HTML and extract information from a website. Here is a simple example that demonstrates how to use Beautiful Soup to extract all the links from a web page:

``from bs4 import BeautifulSoup
import requests

# Make a GET request to the website
response = requests.get('http://www.example.com')

# Parse the HTML of the website
soup = BeautifulSoup(response.text, 'html.parser')

# Extract all the links from the page
links = soup.find_all('a')

# Print the links
for link in links:
    print(link.get('href'))``
    
 Beautiful Soup provides many other useful methods for parsing HTML and extracting information from a website. You can read more about it in the official documentation: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
