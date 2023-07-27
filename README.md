# Apartment Search Script Demo

## Overview
This project is a demo for an apartment search script developed in Python 3.9. It utilizes the requirements specified in the `requirements.txt` file. The script is built on top of the Selenium library and other necessary dependencies. Its primary function is to scrape all available apartments in Berlin from the website https://www.deutsche-wohnen.com/.

## Motivation
The main reason for creating this apartment search script is to address the high competition for affordable apartments in Berlin. The process of finding an apartment in the city can be extremely challenging, often requiring applicants to wait for extended periods. This tool automates the application process for all available apartments listed on the https://www.deutsche-wohnen.com/ website.

## How It Works
The script works by scraping the website to gather information about the available apartments in Berlin. It then stores the details in a dictionary, where each apartment's link is used as the key and the corresponding value is set to a boolean (defaulting to false). This boolean value serves as a flag to indicate whether an application has been sent for a particular apartment.

To ensure efficiency and avoid sending duplicate applications, the script uses the dictionary to track the contacted offers. If the script is run multiple times, it will not resend applications for the apartments that have already been processed.

Please note that, as a demo version, the script only simulates filling out the application form and **does not actually send** the applications.

## Default User
The default user in this demo is "Max Mustermann." However, the script can be easily modified to accommodate different users or allow user input for customization.

## Data Persistence
The script utilizes pickling to store and retrieve the dictionary with apartment details. Pickling is a straightforward way to serialize Python objects, enabling data to be saved and later restored, thus maintaining the history of contacted apartments across multiple script runs.

## Requirements
To run the apartment search script, make sure you have Python 3.9 installed on your system. Additionally, install the required libraries by running the following command in your terminal or command prompt:

<div align="center">

## `pip install -r requirements.txt`

</div>

## Usage
1. Clone or download this repository to your local machine.
2. Install the required dependencies as described in the "Requirements" section.
3. Run the script `apartment_search_script.py` to initiate the scraping process.
4. Observe the script's output to view the details of available apartments.
5. As this is a demo, the script will not send actual applications but will simulate the filling out of the form.

Feel free to modify the script or integrate it into your own projects to suit your specific needs.

**Note**: Please use this script responsibly and with respect to the website's terms of use. Avoid excessive scraping, as it may put strain on the server and violate the website's policies. Always be considerate of others who might also be using the website's resources for legitimate purposes.
