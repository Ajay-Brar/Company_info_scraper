# Company_info_scraper

## libraries
### backend file modules
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.edge.service import Service
from selenium.webdriver.edge.options import Options
from selenium.webdriver.support.ui import WebDriverWait
from selenium.webdriver.support import expected_conditions as EC
from urllib.parse import quote
import time
import pandas as pd
from pathlib import Path

### frontend file modules
import streamlit as st
import pandas as pd
from pathlib import Path
import sys
import os

## Images of working app
![image](https://github.com/user-attachments/assets/0380370d-6657-4b71-9a51-3ce36e020e3f)

![image](https://github.com/user-attachments/assets/3ad55137-b9b3-4f89-bd7b-8312cc486ef9)

## scrapping
Click onn the start button below 
it will start the backend file and start searching from the google map 
then after the search completion it will show you the data in table form
