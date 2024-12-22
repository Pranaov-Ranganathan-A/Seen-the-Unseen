# Seen-the-Unseen
# Web Scraping: Episodes of "Seen & Unseen" (2024)

## Project Overview
This project involves scraping the episode titles of the 2024 season of "Seen & Unseen" from the website using **Python** and **BeautifulSoup**. 

## Project Process

1 **Fetching the Webpage Content**
  import requests
  url = 'https://seenunseen.in/episodes/2024/'
  html = requests.get(url)

2 **Parsing HTML Content with BeautifulSoup**
  from bs4 import BeautifulSoup
  soup = BeautifulSoup(html.content, 'html.parser')

3 **Extracting Episode Titles**
  results = soup.find(id='content')
  episode_title = results.find_all('h2', class_='entry-title')

4 **Save outputs into a pandas DataFrame**
  
