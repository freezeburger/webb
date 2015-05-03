## Webb - Web Scrapper and Crawler
An all-in-one Python library to scrap, parse and crawl web pages

### Gist
This is a light-weight, dynamic and featured Python library. It can be used to **crawl, download, index, parse, scrap and analyze web pages** in a systematic manner or any of the individual function. It is also used to **clean web pages, store web data and import/export relevant components** from the internet. Some of the other features also include **downloading google images and spidering wikipedia articles**.

### Compatability
This library is compatible with both Python 2 (2.x) as well as Python 3 (3.x) versions. It is a download-import-and-run program with no or little changes as required by users.

### Dependencies
There are **no dependencies** to this project. It functions entirely of the standard in-build library support. It does not need any external support or installations. Just download and run!!!

### Usage
1. Download `webb.py`
2. Create a new file in the same folder and give it any name like `main.py`
3. Import the webb library by writing `import webb` in the `main.py` file
4. Once this is done, use any of the following commands

* Traceroute a URL:  
`webb.traceroute("your-web-page-url")`

* Get IP address of a webpage:  
`webb.get_ip("your-web-page-url")`

* Download entire HTML page:  
`print(webb.download_page("your-web-page-url"))`

* Normalize URL (Convert Relative URL to absolute URL):  
`print(webb.url_normalize("your-relative-url","your-seed-page-url"))`

* Print the page title:  
`webb.title("your-web-page-url")`

* Find all the links in a web page and print it one below the other:  
`webb.find_all_links("your-web-page-url")`

* Find all the URLs in a page and convert them into absolute URLs and print it
`webb.find_all_links("www.zseries.in","absolute")`

* Find all the links in a pirticular web page and print it as a list:  
`print(webb.find_all_links_as_list("your-web-page-url"))`

* Get all the headings (h1 or h2 or ... h6) from a given web page and print it one below the other:  
`get_all_headings("your-web-page-url","h1")`

* Get all the headings (h1 or h2 or ... h6) from a given web page and print it as list: 
`get_all_headings("your-web-page-url","h2","list")`

* Get all paragraphs of a given web page one below the other:  
`webb.get_all_paragraphs("your-web-page-url")`

* Get all paragraphs of a given web page one below the other:  
`print(webb.get_all_paragraphs_as_list("your-web-page-url"))`

* Get links of all the images in a given web page:  
`webb.get_all_images("your-web-page-url")`

* Get links of all the images in a given web page and download all those images on local disk (computer):  
`webb.get_all_images("your-web-page-url","download")`

* Clean an HTML page by removing all the HTML tags:  
`print(webb.pure_text("your-web-page"))`

* Crawl web pages in breathe-first manner (Out-of-domain mode):  
`webb.web_crawl("your-web-page-url")`

* Crawl web pages with delay of 2 seconds after every page crawled (Out-of-domain mode):  
`webb.web_crawl("your-web-page-url",2)`

* Crawl an entire website with no (0 seconds) delay while writing the crawl data into a log file (Out-of-domain mode):  
`webb.web_crawl("your-web-page-url",0,"write_log")`

* Crawl web pages in breathe-first manner (In-domain mode):  
`webb.web_crawl_in_domain("your-web-page-url")`

* Crawl web pages with delay of 2 seconds after every page crawled (In-domain mode):  
`webb.web_crawl_in_domain("your-web-page-url",2)`

* Crawl an entire website with no (0 seconds) delay while writing the crawl data into a log file (In-domain mode):  
`webb.web_crawl_in_domain("your-web-page-url",0,"write_log")`

* Download Google Images from keywords or list, as a list output:
`webb.download_google_images("keyword")`  or `webb.download_google_images(['keyword 1','keyword 2','keyword 3'])`

* Download Google Images from keywords to local hard drive:  
`webb.download_google_images('keyword','download')`


### Status
This is a stand-alone python script which is ready-to-run, but still under development. Many more features will be added to it shortly.

### Disclaimer
The crawler function lets you download  and crawl tons of web pages. Please do not download and crawl any pages of a domain without reading about the robot.txt file of that domain. 

It is inappropriate to violate the robot.txt file. This may even lead to the domain completely blocking your crawler and thus blacklisting it. It is also not appropriate to crawl pages at high rate as it may put a lot of pressure on the server.
