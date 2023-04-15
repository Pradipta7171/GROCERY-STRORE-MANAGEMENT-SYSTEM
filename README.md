# GROCERY-STRORE-MANAGEMENT-SYSTEM

The given code is a Java program that implements a simple grocery management system. The program allows users to add grocery items to different categories, delete items, display all items and their details, and buy items by specifying the quantity they want to purchase.

 The main class in the program is GroceryManagementSystem. 

It has the following fields: 
1.	FILENAME: a constant string representing the file name where the grocery items will be stored and loaded from. 

2.	groceryItems: a Map object that stores the grocery items. The map has a string key representing the category of items, and the corresponding value is another map that has string keys representing the name of the item, and a list of strings as the value, containing the item's price, quantity, and unit. 
The GroceryManagementSystem class has the following methods: 
a.	getGroceryItems(): a getter method for the groceryItems field. 

b.	GroceryManagementSystem(): a constructor that initializes the groceryItems field with an empty HashMap, and then loads the grocery items from the FILENAME.


c.	addGroceryItem(String category, String item, double price, String quantity, String unit): a method that takes the category, name of the item, price, quantity, and unit of the item as parameters, creates a new List object containing these details, and then adds this list to the map corresponding to the given category. It also saves the grocery items to the FILENAME after adding the new item. 

d.	deleteGroceryItem(String category, String item): a method that takes the category and name of the item to be deleted as parameters, removes the corresponding entry from the map, and then saves the grocery items to the FILENAME. 
e.	displayGroceryItems(): a method that prints out all the grocery items and their details, categorized by their category, to the console.

f.	buyGroceryItem(String category, String item, int quantity): a method that takes the category, name of the item to be purchased, and the quantity to be purchased as parameters, reduces the quantity of the item in the map by the purchased quantity, calculates the total cost of the purchase, and then prints out a message showing the total cost of the purchase. If the requested quantity is greater than the available quantity of the item, the method will output an error message indicating that there are not enough items in stock. 
The GroceryManagementSystem class also has two private methods:
•	loadGroceryItems(): a method that reads the grocery items from the FILENAME and populates the groceryItems map accordingly. 

•	saveGroceryItems(): a method that saves the current grocery items in the groceryItems map to the FILENAME. 


The GroceryStoreManagement class is a test class that creates a new GroceryManagementSystem object, and then tests the various methods of the GroceryManagementSystem class by calling them with different parameters.



