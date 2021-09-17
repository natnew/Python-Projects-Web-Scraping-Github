# Python-Projects-Web-Scraping-Github 🐍
Python Script <br>
This repo contains python code that scrapes Github pages and returns a Github link to the profile picture. <br>
Run the code.

Python
```python
import requests
from bs4 import BeautifulSoup as bs

github_user = input('Input Github user: ')
url = 'https://github.com/' + github_user
r = requests.get(url)
soup = bs(r.content, 'html.parser')
profile_image = soup.find('img', {'alt': 'Avatar'})['src']
print(profile_image)
    '''
    The shuffle method shuffles the cards.
    '''


    def deal(self, no_of_cards):
        dealt_cards = []
        for i in range(no_of_cards):
            dealt_card = self._cards.pop(0)
            dealt_cards.append(dealt_card)
        return dealt_cards
'''Deals the cards.'''
    def __repr__(self):
        cards_in_deck = len(self._cards)
        return "Deck of " + str(cards_in_deck) + " cards"
        
deck = Deck()
print(deck)
```

Output
```
Input Github user: 
https://.......
```
