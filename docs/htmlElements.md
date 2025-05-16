# htmlElements

The ```htmlElements``` script was pulled out of the ```dicli``` script in the 
[domible project](https://joeldodson.github.io/domible).
It is the core motivation for this WebDevAccess project.
It has dependencies domible does not.
I could add those as optional dependencies for domible but could not configure dicli to be installed optionally.
If you pip installed domible, you'd end up with an installed script, dicli, which failed due to missing dependencies.


```htmlElements``` uses the python requests and beautifulsoup4 packages to get and scrape information from the 
[Mozilla Developers Network (MDN)](https://developer.mozilla.org/).
It creates two tables with references for HTML elements, one for current elements, one for deprecated.
The tables have a row for each element created by scraping the reference page for that element.
It's entirely possible the layout of the reference page on MDN changes and ```htmlElements``` breaks.
If so, please open a ticket on the 
[WebDevAccess issues page](https://github.com/joeldodson/webdevaccess/issues).
