# Navigate Page Post Aria

This will help to Navigate Page Post Aria using the keyboard tab.

```text
def navigatePagePostAria():
    driver.get("https://www.facebook.com/sushen.biswas/")
    driver.implicitly_wait(5)
    actions.send_keys(Keys.BACK_SPACE)
    actions.send_keys(Keys.TAB * 56)
    actions.send_keys(Keys.ENTER)
    actions.perform()
    print(input("Press any Key: "))
```

