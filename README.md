# grocery_store_management_system_oops


This program simulates the operations of a grocery store, where there are two main user roles: **Admin** and **Staff**. The Admin has full access to managing employees, finances, and business operations, while the Staff can handle inventory management, process sales, and request leaves. The system is designed using object-oriented programming principles, with classes and functions organizing the various tasks.

The program is divided into different classes that represent the functionalities required for the store:

1. **Validity Class**: This class provides helper functions, like converting a character or a string to lowercase. This is important for handling user inputs in a consistent way, as the program checks for item names, staff names, and other inputs in a case-insensitive manner.
   
2. **Staff Class**: The Staff class manages the store’s inventory and processes sales. It has functions to add new items to the inventory, adjust the quantities of existing items, and display stock information. It also handles the billing process when items are sold to customers. The Staff class keeps track of cost prices, selling prices, and item quantities.
   
3. **Manager/Admin Class**: The Manager class inherits from the Staff class and adds the ability to manage employees. Admins can add new staff members, view a list of all employees, and calculate the store’s financial standing by determining the net profit and expenditure. The Manager class also allows calculating employee leaves and adjusting their salaries accordingly.

### How will the Program Run

The program operates through a **text-based menu system**. When the program starts, users are first prompted to log in. Based on their choice, they are directed to either the Admin menu or the Staff menu, where they can perform different operations.

### Login Page

The program starts with a **login screen** where users are given three options:

1. **Admin Login**
2. **Staff Login**
3. **Exit**

To log in as an Admin, users need to enter the correct username and password. The Admin's username is **grocery** and the password is **1234**. If the credentials are correct, the Admin gains access to the Admin menu.

### Admin Menu

After logging in as Admin, the following options are available:

1. **Manage Employees**: Admin can add new staff members and view the current employee list.
2. **Net Expenditure**: Admin can view the store’s profit by subtracting the cost of goods sold from the selling price, and also see the net income after deducting employee salaries.
3. **Back to Login Page**: Admin can return to the login screen.

### Staff Menu

When a staff member logs in, they are presented with the following options:

1. **Scan Goods**: This allows the staff member to manage the inventory. They can:
   - Add new items to the stock.
   - Increase the quantity of existing items.
   - Decrease the quantity of items if some are sold or removed.
   - Show the current stock of items.
   - Go back to the Staff menu.

2. **Billing**: This option allows staff to process sales transactions. When customers buy items, the staff can input the item names and quantities, and the program will calculate the bill based on the selling prices and update the stock accordingly.

3. **Take Leave**: Staff can request leaves, and the system will deduct their salary based on the number of days they take off.

4. **Back to Login Page**: Staff can log out and return to the main login page.

### Scan Goods Submenu

Within the **Scan Goods** section, the staff has more specific options to manage the inventory:

1. **Add New Item**: Staff can add a new product to the inventory by entering the item name, cost price, selling price, and quantity.
2. **Increase Quantity of Existing Item**: Staff can add more units of an item to the inventory.
3. **Decrease Quantity of Existing Item**: Staff can reduce the stock of an item, which would usually happen when the items are sold.
4. **Show Stock**: Displays a list of all items in the inventory with their quantities and prices.
5. **Back to Staff Menu**: Returns to the main Staff menu.

### Key Functionalities and Flow

- **Admin Features**: The Admin has full control over the employee management and store finances. They can add new staff, view the list of employees, and calculate the store’s profit and net income. The Admin’s responsibilities include overseeing the overall business operations, making sure the store runs smoothly, and ensuring that employees are paid appropriately after leaves are deducted.
  
- **Staff Features**: Staff members handle day-to-day operations like managing stock, updating item quantities, and processing sales transactions. They are responsible for the inventory, ensuring that products are available in sufficient quantities, and providing customers with correct billing details.

- **Leave Management**: Both Admin and Staff can manage leave requests. The Admin can set the leave allowances for employees, while the Staff can request leaves, which will reduce their salary based on the number of days taken off.

- **Financial Management**: The Admin can view the **Net Expenditure** by calculating the profit made from sales, deducting the costs of goods sold, and subtracting the total staff salaries. This helps to evaluate the overall profitability of the store.

### Example Walkthrough

1. **Login Screen**: The user is asked to select between Admin or Staff login. To log in as Admin, they would need to input the correct credentials: **Username: grocery** and **Password: 1234**.

2. **Admin Menu**: After a successful login, the Admin can choose to manage employees, calculate net expenditure, or return to the login page.

3. **Staff Menu**: After logging in as Staff, the menu options are available for managing goods (e.g., adding items, updating quantities) and processing sales. Staff can also take leave, which will affect their salary.

4. **Billing**: When a sale occurs, the Staff member can enter the product name, the quantity purchased, and the system will calculate the bill and update the stock.

### Summary
This program provides a simple, functional way for a grocery store to manage its employees, inventory, and sales. It allows both the Admin and the Staff to perform different tasks, from managing stock and calculating sales to handling leave requests and employee salaries. The use of classes and functions makes the code organized and easy to understand.
