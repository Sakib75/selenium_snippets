## Select a Chrome Profile
Make sure to close other chromedrivers.
```
from selenium import webdriver
import getpass
  
options = webdriver.ChromeOptions() 
options.add_argument("start-maximized")
options.add_argument(r"--user-data-dir=C:\Users\{}\AppData\Local\Google\Chrome\User Data".format(getpass.getuser()))
driver = webdriver.Chrome(options=options)
driver.get("https://www.google.com/")
```
