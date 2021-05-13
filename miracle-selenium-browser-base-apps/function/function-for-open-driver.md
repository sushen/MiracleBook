# Function for open driver

```text
from selenium import webdriver

def driver():
    global driver
    driver = webdriver.Chrome("./chromedriver.exe", chrome_options=chrome_options)
    #driver.get("https://facebook.com")
```

