# Navigate Page Post Aria

This will help to Navigate Page Post Aria using the keyboard tab.

```text
from selenium.webdriver.common.action_chains import ActionChains
from selenium.webdriver.common.keys import Keys

def navigatePagePostAria():
    driver.get("https://www.facebook.com/sushen.biswas/")
    driver.implicitly_wait(5)
    actions.send_keys(Keys.BACK_SPACE)
    actions.send_keys(Keys.TAB * 56)
    actions.send_keys(Keys.ENTER)
    actions.perform()
    print(input("Press any Key: "))
```



**Better Approach** 

```text
from selenium.webdriver.common.action_chains import ActionChains
from selenium.webdriver.common.keys import Keys

def navigatePagePostAria():
    sleepTime = 4
    for i in range(2):
        driver.implicitly_wait(10)
        actions.send_keys(Keys.BACK_SPACE)
        actions.send_keys(Keys.TAB * 10)
        time.sleep(sleepTime)
        actions.perform()
        print("Firast 10 tabs Working")

    actions.send_keys(Keys.TAB * 6)
    actions.send_keys(Keys.ENTER)
    actions.perform()
    print("Navigate Post area Successfully ")
```

