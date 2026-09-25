# 🎬 100 Movies That You Must Watch

A Python web scraping project that collects a list of the **100 greatest movies** from an archived Empire Online webpage and saves the movie titles into a text file.

This project was built to practice the basics of **web scraping with Python**, especially using the `requests` library to retrieve webpage content and `BeautifulSoup` to extract specific information from HTML.

---

## 📌 Project Overview

The objective of this project is to scrape movie titles from a webpage containing Empire Online's list of the best movies.

Instead of directly scraping the current Empire Online website, this project uses a specific **Internet Archive Wayback Machine URL**. This makes the webpage structure consistent and allows the scraper to reliably find the movie titles.

The Python program:

1. Sends a request to the archived webpage.
2. Receives the webpage's HTML content.
3. Parses the HTML using BeautifulSoup.
4. Finds the HTML elements containing movie titles.
5. Extracts the text from those elements.
6. Reverses the scraped list.
7. Writes the movie titles into a `movies.txt` file.

The project instructions specifically recommend using the archived webpage so that the HTML structure matches the expected solution. :chatgpt-content-reference{index="0"}

---

## 🎯 Objective

The main objective of this project is to learn how to use Python for basic web scraping.

More specifically, the project focuses on:

- Sending HTTP requests
- Retrieving HTML from a webpage
- Parsing HTML
- Finding specific HTML elements
- Extracting text from HTML
- Working with Python lists
- Reversing lists
- Creating and writing to text files

The original project objective is to scrape the top 100 movies and generate a `movies.txt` file containing the movie titles in ascending order. :chatgpt-content-reference{index="1"}

---

## ✨ Features

- 🌐 Scrapes data from a real webpage
- 📦 Uses the `Requests` library
- 🥣 Uses `BeautifulSoup` for HTML parsing
- 🎬 Extracts movie titles automatically
- 🔄 Reverses the scraped list
- 📄 Creates a `movies.txt` file
- 💻 Runs directly from the terminal
- 🕰️ Uses an archived webpage for consistent scraping
- 🐍 Written completely in Python

---

## 🛠️ Technologies Used

### Python

The entire project is written in Python.

Python is used for:

- Sending HTTP requests
- Processing HTML
- Extracting movie titles
- Manipulating the movie list
- Creating and writing to the output file

### Requests

The `requests` library is used to send an HTTP GET request to the archived webpage.

📌 Project Workflow
                ┌─────────────────────┐
                │  Archived Web Page  │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │  requests.get(URL)  │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │    HTML Response    │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │    BeautifulSoup    │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │ Find h3.title Tags  │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │ Extract Movie Text  │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │ Reverse Movie List  │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │     movies.txt      │
                └─────────────────────┘


```python
response = requests.get(URL)
