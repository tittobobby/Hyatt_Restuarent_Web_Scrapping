# Hyatt_Restuarent_Web_Scrapping


 The goal of this project would be to scrape the data from the website :
 "https://www.hyattrestaurants.com/en/dining/india/kochi/malabar-caf%C3%A9-restaurant-menu#5f322c618741d25d205fdf52" and convert it into a CSV file that can be used for later analysis.
 
Malabar Café is a modern and relaxed South Indian restaurant located at the Grand Hyatt Kochi in Mulavukad, Bolgatty. The café draws inspiration from the city's rich culinary and cultural heritage and offers a unique dining experience with a menu featuring traditional Kerala dishes made with age-old recipes, infused with the flavors of Malabar spices.

This script web scrapes the menu of Malabar Cafe restaurant at Hyatt in Kochi, India using the requests, BeautifulSoup, and Selenium libraries.

The script first loads the website URL and uses the requests.get function to store the content of the website to a variable 'data'. It then creates a variable 'driver' and stores the chromedriver path to this variable to automate the creation of a new window with Selenium's driver. It then scrolls to the end of the page to ensure all information is captured, and rate-limits requests after 2 seconds.
After reading the file, it parses the content of the file and stores it in variable 'hyatt_full_data'. It then manually inspects the Hyatt Malabar Cafe website to study the structure of the website to scrape data. After inspection, it finds that all menu information is contained within a div with a class called 'listing_content' and uses that to extract name description and price of each dish on their menu. It creates an empty list to store the data, then loops through each item extracting name description and price of each dish. Finally creates a DataFrame from lists; saving it into csv file


