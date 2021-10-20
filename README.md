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
    

Output
```
Input Github user: 
https://.......
```
