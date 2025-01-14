# Inventory-Management-System
Introduction

The Inventory Management System is a Python-based application designed to streamline the process of managing inventory for a store or warehouse. It provides functionalities for adding, editing, and deleting products, tracking inventory levels, and generating reports. The system integrates user authentication, data validation, and a graphical user interface (GUI) for enhanced usability.

Features

Core Functionalities

Add Product: Users can add new products to the inventory by providing a unique product ID, name, quantity, and price.

Edit Product: Existing products can be updated with new details such as name, quantity, or price.

Delete Product: Products can be removed from the inventory by specifying the product ID.

Low Stock Alerts: The system identifies products with quantities below a specified threshold (default: 10).

Generate Report: A comprehensive report of all products in the inventory is generated, displaying product ID, name, quantity, and price.

Additional Features

User Authentication: Ensures that only authorized personnel can access the inventory system.

Data Validation: Validates inputs such as product ID, quantity, and price to prevent errors.

Graphical User Interface (GUI): Built using Tkinter, the GUI offers an intuitive and user-friendly experience.

System Design

Modules

InventoryManager Class: Handles core functionalities such as adding, editing, and deleting products, as well as generating reports and low-stock alerts.

InventoryApp Class: Implements the GUI and interacts with the InventoryManager class.

Data Structure

The system uses a dictionary to store product details. Each product ID serves as a unique key, and the value is another dictionary containing the product's name, quantity, and price.

Example:

{
    "P001": {"name": "Widget", "quantity": 50, "price": 19.99},
    "P002": {"name": "Gadget", "quantity": 10, "price": 29.99}
}

Validation

Ensures product ID uniqueness when adding new products.

Validates numerical inputs for quantity and price.

Prevents empty or invalid inputs in all fields.


Implementation

Technologies Used

Programming Language: Python

GUI Framework: Tkinter


Code Structure

The code is divided into two main classes:

InventoryManager: Implements the backend logic.

InventoryApp: Handles the frontend and user interactions.



The application is executed using:

if __name__ == "__main__":
    root = tk.Tk()
    app = InventoryApp(root)
    root.mainloop()

User Guide
Launch the application by running the script.


Use the GUI to:

Add new products by entering details in the provided fields.

Edit existing products by specifying the product ID and updated details.

Delete products by entering the product ID.

View low-stock alerts.

Generate and view a complete inventory report.


Testing

The application has been tested for:

Adding products with valid and invalid inputs.

Editing and deleting products with existing and non-existing IDs.

Generating accurate reports and low-stock alerts.


Conclusion

The Inventory Management System simplifies inventory handling by providing a robust and user-friendly solution. The integration of a GUI enhances usability, making it accessible even to users with minimal technical expertise. This application is suitable for small to medium-sized stores or warehouses.
