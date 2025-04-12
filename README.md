# 🌐 Selenium Google Search Bot

This project demonstrates a basic use of [Selenium WebDriver](https://www.selenium.dev/) to automate a browser and perform a Google search.

## 🚀 Features

- Launches a Chrome browser window
- Navigates to [Google](https://www.google.com)
- Enters a search query: `"Hello, World!"`
- Submits the search form
- Waits for the results to load
- Closes the browser

## 🧰 Requirements

- Python 3.x
- [Selenium](https://pypi.org/project/selenium/)
- ChromeDriver (or the appropriate driver for your browser)

## 📦 Installation

1. Install Selenium:
   ```bash
   pip install selenium
   
## 📝 Code Overview
```python
from selenium import webdriver
from selenium.webdriver.common.by import By

driver = webdriver.Chrome()
driver.get("https://www.google.com")
search_box = driver.find_element(By.NAME, "q")
search_box.send_keys("Hello, World!")
search_box.submit()
driver.implicitly_wait(5)
driver.quit()
```
##❗ Notes
* If you’re using Firefox or another browser, use the appropriate WebDriver like `webdriver.Firefox()`.
* You can customize the search term by changing the send_keys() input.
