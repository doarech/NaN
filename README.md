from selenium import webdriver
from selenium.webdriver.common.by import By
import time


driver = webdriver.Chrome()


driver.get("https://chatgpt.com")

time.sleep(3)


input_element = driver.find_element(By.ID, "prompt-textarea")

time.sleep(3)


input_element.send_keys("Merhaba")

time.sleep(3)

input_element.send_keys(Keys.ENTER)


time.sleep(3)
