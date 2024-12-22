# Seen-the-Unseen
# Web Scraping: Episodes of "Seen & Unseen" (2024)

## Project Overview
This project involves scraping the episode titles of the 2024 season of "Seen & Unseen" from the website using **Python** and **BeautifulSoup**. 

## Project Process

**Fetching the Webpage Content**
import requests
url = 'https://seenunseen.in/episodes/2024/'
html = requests.get(url)

**Parsing HTML Content with BeautifulSoup**
from bs4 import BeautifulSoup
soup = BeautifulSoup(html.content, 'html.parser')

**Extracting Episode Titles**
results = soup.find(id='content')
episode_title = results.find_all('h2', class_='entry-title')
episode_list = [episode.text.strip() for episode in episode_title] 
