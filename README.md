# Data-Science-From-Scratch

##Reading Files

By using stdin and stdout it's easy to create unix like utilities for text processing and pipe them into each other. For example, to count the number of lines in a file that contain numbers:

```
cat someFile.txt | python egrep.py "[0-9]" | python line_count.py 
```

##Web Scraping

Be sure you've set up a virtual environment and then just use BeautifulSoup, Requests and html5lib.

```python
source_code_of_a_webpage = BeautifulSoup(requests.get(url_of_page).text,'html5lib')
```
