# SI507-Final

This is a restaurant recommendation application based on the location. 

The program uses Yelp fusion API to get restaurant information. The program uses Google Maps API to get the user's current location. The program gives you two options to search restaurants:
  1. The user can manually type the city name in the form and the program will show you the recommended restaurant list around typed area. The program accepts the abbreviation and can modify the typo if it's understandable.
  2. The user can click "Go" button to get the recommended restaurant list based on their current location.
  
- HOW TO RUN THE CODE  
To run the program, please install all required python packages, change into the directory where you store the python and data file, and run the python file. After running "final.py" code, since I used Flask for interaction, go to localhost:5000 in your web browser and please interact with the features. It will show you restaurant recommendations in a table format. You can get more information of the restaurant by clicking on “More Info” Link on each restaurant. It will bring you to the Yelp website about each restaurant. 

- PACKAGES
equests, flask, googlemaps

- DATA STRUCTURE 
The basic data structure is a dictionary structure. I made an unrooted tree (dictionary) with each restaurant's information. Nodes are name, rating, price, image url, and url. The search_term(search city) will be a key for the cache. The searched result will be separated by each restaurant. For each restaurant, a dictionary will be defined, and the features (such as rating, price, url) that I’m interested in will be the keys to the dictionary. The information of each creature will be a value for each key in the dictionary. And then, each dictionary will be saved as a cache to be reused.
