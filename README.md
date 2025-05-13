🛒 𝐈𝐧𝐯𝐞𝐧𝐭𝐨𝐫𝐲 𝐌𝐚𝐧𝐚𝐠𝐞𝐦𝐞𝐧𝐭 𝐒𝐲𝐬𝐭𝐞𝐦

This is a command-line based Inventory Management System written in Python that allows users to manage a collection of products across different categories: Electronics, Grocery, and Clothing. The system supports CRUD operations, inventory valuation, data persistence with JSON, and more.

📦 𝐅𝐞𝐚𝐭𝐮𝐫𝐞𝐬

- Add new products to inventory (Electronics, Grocery, Clothing)
- Sell products and reduce stock quantity
- Restock existing products
- Search products by name or type
- View all products in inventory
- Remove expired grocery items
- View total inventory value
- Save and load inventory data from a JSON file
- Exception handling for:
  - Duplicate product IDs
  - Selling out-of-stock items
  - Invalid product data

🧱 𝐏𝐫𝐨𝐝𝐮𝐜𝐭 𝐓𝐲𝐩𝐞𝐬

1. Electronics
- Product ID
- Name
- Price
- Quantity
- Warranty Years
- Brand

2. Grocery
- Product ID
- Name
- Price
- Quantity
- Expiry Date (YYYY-MM-DD)

3. Clothing
- Product ID
- Name
- Price
- Quantity
- Size
- Material

📂 𝐅𝐢𝐥𝐞 𝐒𝐭𝐫𝐮𝐜𝐭𝐮𝐫𝐞

- Product (Abstract Base Class)
- Electronics, Grocery, Clothing (Subclasses)
- Inventory (Manages collection of products)
- main() (CLI menu for user interaction)
- JSON I/O for saving and loading inventory data


🧰 𝐃𝐞𝐩𝐞𝐧𝐝𝐞𝐧𝐜𝐢𝐞𝐬

- No external libraries required.
- Uses only standard Python libraries:
  - json
  - abc
  - datetime

❗ 𝐂𝐮𝐬𝐭𝐨𝐦 𝐄𝐱𝐜𝐞𝐩𝐭𝐢𝐨𝐧𝐬

- OutOfStockError: Raised when selling more than the available quantity.
- DuplicateProductError: Raised when adding a product with an existing ID.
- InvalidProductDataError: Raised during JSON loading if product data is invalid.

📌 𝐍𝐨𝐭𝐞𝐬

Grocery items are automatically flagged and removed if expired.
Product details are preserved in JSON format, including subclass-specific attributes.
The system is modular and can be extended to support more product types or persistence methods (e.g., databases).


Developed by Ayesha Nadeem 
