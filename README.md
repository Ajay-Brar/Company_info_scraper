# Dynamic Info Scraper (Google Maps)
## Images of working app
![image](https://github.com/user-attachments/assets/0380370d-6657-4b71-9a51-3ce36e020e3f)

![image](https://github.com/user-attachments/assets/3ad55137-b9b3-4f89-bd7b-8312cc486ef9)

## scrapping
Click onn the start button below 
it will start the backend file and start searching from the google map 
then after the search completion it will show you the data in table form


A dynamic web scraping application built with **Streamlit** and **Selenium** that allows users to extract company details (Name, Address, and Phone Number) from Google Maps based on custom search queries.

## Features

* **Interactive UI:** User-friendly interface built with Streamlit for entering search queries.
* **Automated Scraping:** Uses Selenium with the Microsoft Edge WebDriver to navigate Google Maps and extract data in real-time.
* **Data Persistence:** Automatically saves scraped results to a CSV file (`company_data.csv`) and displays existing data on launch.
* **Visual Feedback:** Shows the scraping progress and results directly within the web app.

## Prerequisites

* **Python 3.x**
* **Microsoft Edge Browser** installed on your system.

## Installation

1.  **Clone the repository** (or ensure all source files are in the same directory).

2.  **Install Required Packages**
    Run the following command to install the necessary Python libraries:
    ```bash
    pip install streamlit pandas selenium webdriver-manager
    ```

## Usage

1.  **Run the Application**
    Navigate to the project directory in your terminal and execute:
    ```bash
    streamlit run app.py
    ```

2.  **Using the Scraper**
    * The application will open in your default web browser (usually at `http://localhost:8501`).
    * Enter a search term (e.g., "Software companies in California") in the input field.
    * Click **Start Search**.
    * The app will launch a headless Edge browser, scrape the data, and populate the table on the screen.

## Project Structure

* **`app.py`**: The main frontend application. Handles user input, displays data, and manages the UI logic.
* **`backend_script.py`**: Contains the Selenium automation logic to scrape Google Maps.
* **`company_data.csv`**: The output file where scraped company details are stored.
* **`ci.png`**: An image asset displayed in the main application interface.

## Troubleshooting

* **WebDriver Issues:** If the automation fails to start, ensure you have Microsoft Edge installed. The script attempts to use `webdriver_manager` to automatically handle the driver. If that fails, download the specific [Edge WebDriver](https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/) for your browser version, rename it to `msedgedriver.exe`, and place it in the project root.

## Disclaimer

This tool is for educational purposes only. Scraping data from websites like Google Maps may violate their Terms of Service. Please use this tool responsibly.
