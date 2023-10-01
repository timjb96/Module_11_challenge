# Martian Analysis: News, Weather, Conditions
# UC Davis Data Analytics Bootcamp Project
Skills Used: Python, Jupyter Notebook, Spark, BeautifulSoup, Pandas, NumPy, MatPlotLib, HTML Reading, AWS

The purpose of this project was to use a webscraper via Beautiful Soup to pull Article information and data from redplanetscience.com.

The first Jupyter Notebook file uses Beautiful Soup to scrape Article information from Redplanetscience.com, specificall Article Titles and Subheadings. 
This is useful as it allows us to pull a report of the most recent bits of news about Mars quickly, and allows us to comb through the articles quicker to find an example of what kind of articles we specifically need at that time. We do this by storing the article titles and descriptions in a dictionary made up of key-value pairs of the title and description. 

![Screen Shot 2023-09-30 at 2 32 50 PM](https://github.com/timjb96/Module_11_challenge/assets/112847821/4c700f0e-04be-46e4-a935-1c61d14a13c8)

This yields the following:

![Screen Shot 2023-09-30 at 2 33 21 PM](https://github.com/timjb96/Module_11_challenge/assets/112847821/410f5971-bda2-4a76-8e4a-962f069a03d4)

From a list like this, we could easily generate further reports about types of news stories, or certain key terms about the articles. This could also be useful in back-end search functions, as a dictionary that a user-input search engine on the website could generate and read through to direct readers to stories based on their search.

The second Jupyter Notebook file uses Beautiful Soup again to pull Mars data from an Amazon AWS website, https://data-class-mars-challenge.s3.amazonaws.com/Mars/index.html.

This analysis is much more focused on data from Mars itself, and we used it to answer several questions about conditions on mars. 

First, we set up a dataframe to show us data regarding temperatures and pressures on Mars over time. Then, we set up a dataframe that allows us to make date-time comparable between earth and mars, so that we can have a meaningful understanding of seasonal trends on the Red Planet. 

![Screen Shot 2023-10-01 at 10 36 01 AM](https://github.com/timjb96/Module_11_challenge/assets/112847821/77329498-b52e-4ef3-9b01-8ef37be4d607)


From here, we are able to plot out the temperatures by Martian Month:

![Screen Shot 2023-10-01 at 10 37 45 AM](https://github.com/timjb96/Module_11_challenge/assets/112847821/9de1f884-5d70-4a57-8c69-7adffba7954d)

We then do the same with the pressures. From here, we also do a similar calculation on Martian Days as we did for months, so that we can determine the daily minimum temperatures over time.

![Screen Shot 2023-10-01 at 10 40 09 AM](https://github.com/timjb96/Module_11_challenge/assets/112847821/271aad48-cb4c-4e65-ba12-ede42c771e6d)

