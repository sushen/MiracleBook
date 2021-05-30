# Validation

This we can validate any Xpath link

```text
def navigateGroupPostBtn():
    grpupPostXpath = "//span[contains(text(),'s on your mind,')]"
    grpupPostX2ndpath = "//span[contains(text(),'Create a public post…')]"

    grpupPostXpathAria = driver.find_elements_by_xpath(grpupPostXpath)
    grpupPost2ndXpathAria = driver.find_elements_by_xpath(grpupPostX2ndpath)

    if driver.find_elements_by_xpath(grpupPostXpath):
        grpupPostXpathAria[0].click()
        print(grpupPostXpath + "is the 1st Xpath and its working")

    elif driver.find_elements_by_xpath(grpupPostX2ndpath):
        grpupPost2ndXpathAria[0].click()
        print(grpupPostX2ndpath + "is the 2nd Xpath and its working")

    else:
        print("Path Not Found")
```

