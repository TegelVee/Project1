# Lede Program, Project 1: Scraping wife carrying

In this my first scraping project, in which I scraped an unordered list from a wife carrying Wikipedia article. https://en.wikipedia.org/wiki/Wife-carrying I did scraping, cleaning and analyzing in VS Code and used e.g. these tools and libraries: pandas, requests, BeautifulSoup, re. See the whole process in my notebook (https://github.com/TegelVee/Project1/blob/main/wifecarrying01.ipynb). 
I wrote a story of my findings (https://tegelvee.github.io/Project1/) that I completed short before deadline manually, when the championship was resolved on July 6, 2024. I used Datawrapper to create two graphics from my analysis. To be able to publish the piece, I needed to use html and css.

Findings
In my analysis I found that by 2024, Finland had won The Wife Carrying World Championships 11 times, as well as Estonia too. Mr. Taisto Miettinen (FIN) has achieved most personal wins. Due to the covid pandemic the competition could not be organized in two years. I also analyzed winning times from all years, and it revealed out, that Estonian Mr. Margo Uusorg is dominating the fastest winning times.

Analysis
After scraping the data with requests, I made a soup object of it, but the data needed a lot of organizing and cleaning. Because there were no clear html elements to use in analysis, I had to split the scraped text in various ways to form a dataframe (df). After getting the df, I cleaned the data with regular expression (re). I had to change one column's datatype and after that save everything into a new df.
When interviewing the data, I used for example value_counts, groupby and tolist.

Learned new skills
Scraping an unordered list (ul)
split function: things can be separated from each other e.g. with punctuation marks (‘ - ‘, ‘ , ‘, ‘ and ‘)
re library https://docs.python.org/3/library/re.html (e.g. re.search(), replace())
getting flags in Datawrapper with country codes https://docs.google.com/spreadsheets/d/1_L2UbOTqwOAAzN3rkjNLeeiR3rSYmUshhj4tP26AJfs/edit?gid=0#gid=0 
html
css

What would I have liked to do more?
Compare the champion data with data about all people who have attended the championships by the years. Probably every year there have been contestants from Germany, USA and Sweden. How bad are their times, because they never got to the championship list? Unfortunately, comprehensive result data does not exist.
Scrape data from this year’s attendees from the official wife carrying page, but had no time, because the competition took place one day before the project deadline. https://eukonkanto.fi/tulokset/ 
Use Illustrator to make scrolly tell or for example a map of the wife carrying track. 
