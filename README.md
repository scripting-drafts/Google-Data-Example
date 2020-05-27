# Google-Data-Science

This scripts are meant to be run on GNU/Linux but can be adapted to OSX by changing CONTROL keys to COMMAND keys.

Requirements:
 - Firefox
 - Geckodriver
 - Python3.7
 
 Libraries:
  - Selenium
  - tqdm
  - CSV
  - Itertools
  - Folium
  - Pandas
  - Branca
  
 # places-to-csv.py
Scraps Barcelona City on Google Maps by neighbourhoods. Asks for a keyword and makes an array with found places names and locations, later on it removes duplicates from the array and searchs for those locations one by one, scraping Name, Address, Stars Rate, Number of Comments, Type of the place and Coordinates (lat, lon). It also makes an 8th column to debug Errors. It ends writing all the information to a CSV file with UTF-8 encoding and semicolon delimiter.
 
 # csv-to-html-map.py
Takes the CSV file as the only argument. Creates a map with markers of all places classifying their Number of Comments by color and their Stars Rate by diameter of the marker.
