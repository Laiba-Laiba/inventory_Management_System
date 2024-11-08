Inventory Management System

This Inventory Management System is built using a Binary Search Tree (BST) where each node represents an item in the inventory. Each item has attributes like item_id, item_name, item_description, quantity, and price. The system supports various inventory operations such as insertion, search, deletion, updating, and management of stock. Additionally, it includes price-based queries and bulk insertion/updating from a text file.


Features and Operations

Item Structure

Each item in the inventory has the following attributes:


item_id: A unique integer identifier used as the key in the BST for maintaining structure.

item_name: The name of the product.

item_description: A brief description of the product.

quantity: The number of units in stock.

price: The cost of a single unit of the product.

Working

Insert an Item:


Add a new item to the inventory using the item_id to maintain the BST order.
Each item is inserted as a node in the BST, with item_id acting as the key.

Search for an Item:

Search for an item by its item_id and return the item's details.
This operation allows quick access to specific items in the inventory.

Delete an Item:


Remove an item from the inventory based on its item_id.
The deletion operation maintains the BST structure after removing the specified item.

Update Item Information:


Update the quantity and price of an item by searching with item_id.
This operation modifies the stock quantity or price of an existing item.

Check Stock Availability:

Verify if a particular item (identified by item_id) is in stock and display the available units.

Low Stock Alert:

Returns a list of items with low stock (e.g., fewer than 3 units).
This alert helps identify items that need restocking.

Restock Item:

Increase the quantity of an item based on user input.
The function takes item_id and a quantity x to add to the item's existing stock.

Find Items within a Price Range:

Returns a list of items within a specified price range [min_price, max_price].
This operation is useful for filtering items based on budget constraints.

Find the Cheapest Item:

Returns the item with the lowest price in the inventory.

Find the Most Expensive Item:

Returns the item with the highest price in the inventory.

Bulk Insertions/Updates from a File:

This feature allows bulk insertion and updating of items from a text file.
The function reads item data from the file and checks if each item already exists in the inventory based on item_id.
If the item is already present, the system updates its attributes if they differ from the current values.
If the item is not present, it inserts the item as a new node in the BST.

Implementation Details

Data Structure: The system uses a Binary Search Tree (BST) where each node represents an item, with item_id used as the BST key.

File Format: Plain text is used for bulk insertion and updating, with each line containing item attributes in a specific format (e.g., item_id, item_name, item_description, quantity, price).


Requirements

A C++ compiler (e.g., GCC) for compiling the program.

A text file for bulk insertions/updates, with each line representing an item and its attributes in the correct format.


Usage Instructions

Compile the Program: Use a C++ compiler to compile the BST-based Inventory Management System.

Run the Program: Execute the compiled program to access the inventory operations.

Perform Operations: Follow the prompts to insert, search, delete, update, or manage stock items.

Bulk Insert/Update from Text File: Use a text file with item data to perform bulk operations.


Example Text File Format

101, "Smartphone", "Latest model with high performance", 15, 699.99

102, "Laptop", "Lightweight and powerful", 7, 1200.00

103, "Tablet", "Portable device with HD display", 3, 299.99


Conclusion

This Inventory Management System provides a structured and efficient way to manage electronic gadgets using a Binary Search Tree. The system's operations allow easy handling of items, including searching, updating, and stock management, with additional features for price-based queries and bulk data handling.






