# Active post area and postin page



```text
from selenium.webdriver.common.action_chains import ActionChains
from selenium.webdriver.common.keys import Keys

def activePostAreaAndPostInPage():
    driver.implicitly_wait(10)
    actions.send_keys(Keys.BACK_SPACE)
    active_post_area = driver.switch_to.active_element
    active_post_area.send_keys("'driver.switch_to.active_element' "
                               "this code is a one of important snippet for facebook automation.")
    actions.send_keys(Keys.TAB * 10)
    actions.send_keys(Keys.ENTER)
    actions.perform()
    print(input("Press any Key: "))
```

**Better Approach** 

```text
from selenium.webdriver.common.action_chains import ActionChains
from selenium.webdriver.common.keys import Keys

def activePostAreaAndPostInPage():
    sleepTime = 4
    implicitlyWaitTime = 20
    time.sleep(sleepTime)

    active_post_area = driver.switch_to.active_element
    driver.implicitly_wait(implicitlyWaitTime)
    time.sleep(sleepTime)
    active_post_area.send_keys("'driver.switch_to.active_element' "
                               "this code is a one of important snippet for facebook automation.")

    actions.perform()
    print("Writing Post in the post area Successfully ")

    for i in range(2):
        driver.implicitly_wait(implicitlyWaitTime)
        actions.send_keys(Keys.TAB * 5)
        print(str(i) + " tabs Working")
    actions.send_keys(Keys.ENTER)
    actions.perform()
```

