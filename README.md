# restaurant-management
This project is a restaurant management system which provides a detailed and useful menu for a Chinese restaurant, Fu King Chinese, which translates to “Deputy King”  in Chinese . 
The aim of this project is to create a database to catalogue the restaurant’s menu into an easily accessible relational database system. Using this database, data can be filtered, related and changed at any moment with ease. 

A frontend application has also been created to access the database’s content , in the form of a GUI supported and hosted by Python using a library called TKinter.
TKinter is a standard GUI library used extensively to create simple and accessible GUIs. Widgets such as buttons, labels and entry boxes can be manipulated with ease. 
A frontend GUI is used to access the database, with many useful assets such as a search bar to search for specific dish names, a price filter to differentiate the menu items by price range, a button toggle that toggles between vegetarian and non-vegetarian items, and a pricing system to easily order and total a customer’s bill. Widgets such as labels, buttons, entry boxes and more have been used to achieve this. 
The project window is split into three frames: a main window, a tree to host the data in a table and a frame to host the table easily. 

A host of suitable images have also been used to appeal to customers. The library PIL has been used to host these images and facilitate easy use with TKinter’s GUI. 
PIL and TKinter are libraries that can easily be used in tandem, which makes PIL the optimal choice for an image based library.

The menu is also complete with 30 authentic Chinese dishes, complete with detailed records of its type, price and more.

***Functionality and Modules***

The project has many features, which include:
Streamlined GUI with buttons, entry boxes and more
Detailed and organised menu system listing item’s nature and price
Search function to search for desired dishes
V/N button to toggle between vegetarian and non-vegetatarian items
Price filter to browse dishes in a specific price range
Streamlined billing system that allows user to easily tally dishes 

GUI
The GUI was built using the library TKinter as a framework. Using a TKinter window, a frame was placed on the window which was used as a platform for the tree which would host the database’s information.

Menu system
The menu system pulls data from an SQL database by using the mysql.connector library to connect to the database. Using insert commands, 30 dishes have been listed, complete with their prices and type. A scroll bar has also been integrated with the table to facilitate scrolling through a limited space to view all the entries.

Search function
Using an SQL query generated by the user’s input in the search field, the specific records are fetched from the database and inserted into the table if the name contains the string of the search function.

V/N Button
A TKinter button widget was used as a toggle for this tool. Upon clicking the button, a counter “yn” is appended by 1 and the correct outcome is decided using the mod function, which can land on 3 states: all items, only veg items and only non-veg items. The all items state makes the button white, the veg state makes the button green and the non-veg state makes the button red.

Price filter
Much similar to the search function, 2 entry boxes have been used to take a lower and higher number as input for the range of the price. Once taken, it is inserted into an SQL query which fetches the applicable records and displays it in the table.

Billing system
This system works on the concept of listing the serial number of the desired dish one at a time. On entering the serial number of the desired dish into the entry box, a check is first run to check if the box is empty or if the serial number exceeds the number of dishes. If the check succeeds, an SQL query is run to fetch the price using the serial number, and the price is sliced from the raw data. It is then incremented to the price counter and appended to a list that displays all the items bought so far. 


<img width="927" alt="Screen Shot 2023-08-05 at 7 40 51 PM" src="https://github.com/deas28/restaurant-management/assets/66839991/5892ae7c-cafe-4ea7-adc4-80779d0427f6"><img width="959" alt="Screen Shot 2023-08-05 at 7 40 57 PM" src="https://github.com/deas28/restaurant-management/assets/66839991/1685325b-2a93-4fac-8e8c-d8b51323b9ca">

<img width="960" alt="Screen Shot 2023-08-05 at 7 41 03 PM" src="https://github.com/deas28/restaurant-management/assets/66839991/b70c0a7e-2ae0-4769-b2d1-00426f9d5192"><img width="968" alt="Screen Shot 2023-08-05 at 7 41 12 PM" src="https://github.com/deas28/restaurant-management/assets/66839991/fdd2556d-a62f-4c5c-806c-fd91191f6d82">
