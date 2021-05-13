# Function for chrome browser

```text
from selenium.webdriver.chrome.options import Options

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
```

