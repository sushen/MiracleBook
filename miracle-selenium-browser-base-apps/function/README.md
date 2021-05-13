# Function

```text
#   Copyright (c) 2021.
#   Version : 0.0.1
#   Script Author : Sushen Biswas
#
#   Sushen Biswas Github Link : https://github.com/sushen
#
#   !/usr/bin/env python
#   coding: utf-8


from selenium import webdriver
from selenium.webdriver.common.action_chains import ActionChains
from selenium.webdriver.chrome.options import Options


def driver():
    global driver
    driver = webdriver.Chrome("./chromedriver.exe", chrome_options=chrome_options)
    driver.get("https://facebook.com")

def chrome_options():
    global chrome_options
    chrome_options = Options()
    chrome_options.add_argument("--start-maximized")
    # chrome_options.add_argument("user-data-dir=chrome-data")
    chrome_options.add_argument('--profile-directory=Default')
    # prefs = {"profile.default_content_setting_values.notifications" : 2}
    # chrome_options.add_experimental_option("prefs",prefs)
    chrome_options.add_argument('disable-infobars')
    chrome_options.add_experimental_option("useAutomationExtension", False)
    chrome_options.add_experimental_option("excludeSwitches", ["enable-automation"])

def actions():
    global actions
    actions = ActionChains(driver)


chrome_options()
driver()
actions()


```

