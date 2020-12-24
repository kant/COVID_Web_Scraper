# COVID Web Scraper

### Contents
1. [Project Intent](#Project Intent)
2. [Data Sources](#Data Sources)
3. [Features](#Features)
4. [Helper Function Explanations](#Helper Function Explanations)

## Project Intent
This web scraping tool collects COVID data from two sources (John Hopkins Github and the COVID Tracking Project), reformats the datetime information, determines what data is new, and appends it into the master dataset.

This web scraper uses two methods for data collection: using the Selenium module and associated Chromedriver to navigate to the COVID Tracking Project website and pull daily case data from their API, and launching a git shell to pull ____ from the Johns Hopkins COVID19 data repo.

This tool was built while at Ford Motor Company for my section's technical specialist Reid.  He was keeping the team up to date on the latest COVID numbers locally and regionally through several Tableau visualizations.  Unfortunately though, the process he was using of manually collecting the data and formatting it properly was consuming a fair amount of his time, especially given that this preprocessing was a once- or twice-weekly process.  Thus, I decided to lend him a hand on this by automating the process, giving me an opportunity to practice my data scraping skills.

## Data Sources
* COVID Tracking Project at the Atlantic - https://covidtracking.com/data/api
* Johns Hopkins COVID-19 Data Repository - https://github.com/CSSEGISandData/COVID-19

## Features
* Directory Check
  * Ensures the user has all the necessary helper files required to run the script and alerts the user through assert statements if a given file is missing from the base directory

## Helper Function Explanations

<details><summary>Functions</summary>
<p>

1. [get_dirs](#get_dirs)
2. [get_todays_date](#get_todays_date)
3. [create_webdriver](#create_webdriver)
4. [get_CTP_data](#get_CTP_data)
5. [get_JH_data](#get_JH_data)
6. [create_JH_master](#create_JH_master)
7. [update_JH_master](#update_JH_master)

</p>
</details>


### get_dirs
This function simply returns the following five directories for use by the other functions in this webscraper:
* root_dir - the root directory on the host machine
* helper_files_dir - the sub-directory containing all the helper files and modules
* downloads_dir - the downloads folder of the host machine
* CTP_data_dir - 
* JH_data_dir - 

### get_todays_date


* current_day
* current_month
  
### create_webdriver
This function does two main jobs:
* Acquiring the version of Chrome currently installed on the host machine
* Creating an instance of the Chromedriver for use in get_CTP_data function

### get_CTP_data
This function does the hard yards of getting the COVID Tracking Project (CTP) data, formatting the filename, moving it to where it needs to be, etc.

### get_JH_data

### create_JH_master

### update_JH_master





