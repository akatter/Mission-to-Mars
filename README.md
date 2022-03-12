# Mission-to-Mars - Module 10 Challenge
Module 10 HTML


## Overview of the Analysis

The purpose of this project was to create a website to distribute Mars data scraped from various sources and create a website using tools including Flask, MongoDB, Beautiful Soup and Splinter.

## Resources Used
- Data Source: 
    - https://data-class-mars.s3.amazonaws.com/Mars/index.html
    - https://data-class-jpl-space.s3.amazonaws.com/JPL_Space/index.html
    - https://data-class-mars-facts.s3.amazonaws.com/Mars_Facts/index.html
    - https://marshemispheres.com/
- Software: Python 3.7.6, Visual Studio Code 1.63.2, Conda 4.11.0, Jupyter Notebook 6.4.6, MongoDB 5.0.6, Beautiful Soup 4.10.0, Splinter 0.17.0

## Results

The results can be obtained by running the app.py file to produce the webpage for analysis, which can be updated by clicking the Scrape New Data button.

To improve functionality, the colour and size of the "Scrape New Data" was adjusted for ease of clicking on smaller devices as well as visibility. This change is represented in the code below:
```
<p><a class="btn btn-info btn-lg btn-block" href="/scrape" role="button">Scrape New Data</a></p>
```

The table was also modified to be compressed in size to better align with the image beside it, which may future proof the table if updated information takes up more space, such as an added description. Highlighting the text where the mouse or finger is hovering was also added, as shown in the code below:

``` 
return df.to_html(classes="table table-hover table-condensed")
```