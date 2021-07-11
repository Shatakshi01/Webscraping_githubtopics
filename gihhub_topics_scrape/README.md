
# Scraping Top Repositories for Topics on GitHub


- We're going to scrape https://github.com/topics
- We'll get a list of topics. For each topic, we'll get topic title, topic page URL and topic description
- For each topic, we'll get the top 25 repositories in the topic from the topic page
- For each repository, we'll grab the repo name, username, stars and repo URL

### Steps to scrape topics and then scrape the top repos from each topic

- use requests to downlaod the page
- user BS4 to parse and extract information
- convert to a Pandas dataframe

### We scrape list of topics with description and URL. Get the top 25 repositories from a topic page
- We have 30 topics in total 
- That means 30 urls 30 titles and 30 descriptions.
- Furthermore, we have scraped top 30 repositiories for each topic
- We have scraped and stores 30 csv files in `data` folder.  

### Once we are done we put it all together
- We have a funciton to get the list of topics
- We have a function to create a CSV file for scraped repos from a topics page

### Libraries Used 
- Pandas
- BeautifulSoup
- requests
- os