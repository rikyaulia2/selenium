from selenium import webdriver
from selenium.webdriver.common.by import By

# Set up the WebDriver (Make sure you have the correct driver installed)
driver = webdriver.Chrome()  # Or use webdriver.Firefox() if using Firefox

# Open a website
driver.get("https://www.google.com")

# Find the search box and enter text
search_box = driver.find_element(By.NAME, "q")
search_box.send_keys("Hello, World!")

# Submit the search
search_box.submit()

# Wait for a few seconds (optional)
driver.implicitly_wait(5)

# Close the browser
driver.quit()
