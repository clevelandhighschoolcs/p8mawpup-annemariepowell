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
https://scontent-sea1-1.xx.fbcdn.net/v/t31.0-8/24799592_507457339624346_3229305495429015185_o.jpg?oh=7980048fca0e1053b360c70cb0bf96b4&oe=5AC9C2E2
