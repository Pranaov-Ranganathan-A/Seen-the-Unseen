# Seen-the-Unseen
# Web Scraping: Episodes of "Seen & Unseen" (2024)

![my banner](https://userimages.githubusercontent.com/75753187/123358567-aac7b900-d539-11eb-8275-0b380264bb4c.png)

## Project Overview
This project aims to scrape the episode titles from the "Seen & Unseen" website for the year 2024 using **Python** and **BeautifulSoup**. The scraped data is then saved into a CSV file for future analysis or record-keeping.

## Project Process

1. **Fetching the Webpage Content**
   - Use the `requests` library to download the HTML content of the target webpage.

   ```python
   import requests

   url = "https://seenunseen.in/episodes/2024/"
   response = requests.get(url)
   html_content = response.text
