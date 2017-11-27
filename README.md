#moo.py

# import libraries

import urllib2

from bs4 import BeautifulSoup

# specify the url

quote_page = 'https://www.zillow.com/home-values/'



page = urllib2.urlopen(quote_page)

soup = BeautifulSoup(page, 'html.parser')

yui_3_18_1_1_1511302438096_2677_box = soup.find('h2', attrs={'id': 'yui_3_18_1_1_1511302438096_2677'})

yui_3_18_1_1_1511302438096_2677 = yui_3_18_1_1_1511302438096_2677_box.text.strip()

print yui_3_18_1_1_1511302438096_2677

# screenshot URL of Command Prompt
http://moodle.clevelandhighschool.org/draftfile.php/5656/user/draft/943409410/i%20TRIED.PNG
