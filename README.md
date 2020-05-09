# web-scraping-marathon_data

The data for the Nashville Rock-and-Roll Marathon that you worked with in Excel was scraped from the `www.runrocknroll.com` race results page. 
Now it's your turn to scrape the data from the website! 
The base URL that you will build out is provided below along with the URL path *per race* and query params.

## URL Config For The RunRockNRoll Website 

Use this to build your urls!
Notice the `&page=` part at the ends..
This is not complete. 
You will need to determine a page number to add to the end of this.

```
MARATHONS_CONFIG = {
    'base_url': 'https://www.runrocknroll.com',
    'query_params': 'gender=&agegroup=&bib=&firstname=&lastname=&page=',
    'pages': [
        'Events/Nashville/The-Races/Marathon/2019-Results',
        'Events/Nashville/The-Races/Marathon/2018-Results',
        'Events/Nashville/The-Races/Marathon/2017-Results',
        'Events/Nashville/The-Races/Marathon/2016-Results',
        'Events/Nashville/The-Races/Half-Marathon/2019-Results',
        'Events/Nashville/The-Races/Half-Marathon/2018-Results',
        'Events/Nashville/The-Races/Half-Marathon/2017-Results',
        'Events/Nashville/The-Races/Half-Marathon/2016-Results'
    ]
}
```

An example URL might look like: 
```
https://www.runrocknroll.com/Events/Nashville/The-Races/Marathon/2019-Results?gender=&agegroup=&bib=&firstname=&lastname=&page=1
```

### Reference
Use the GitHub Webscraping Notebook we walked through in class as a reference on how to approach this. 

Additionally.. 
The RunRockNRoll website _submits a form_ to request data to populate the website. 
In order to fetch the data yourself.. 
What kind of REST action might you use to  with this?

## Next Steps

After loading the marathon and half-marathon data to DataFrames in Python, perform EDA as usual. 
Think of a question that you find interesting and answer it with the data. 
Prepare a brief (5 minutes) presentation to share what you find.

![runners](assets/marathon.jpeg)
