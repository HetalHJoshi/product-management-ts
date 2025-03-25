🛍️ Product Management System
A simple web-based Product Management System built with HTML, CSS, JavaScript, and Bootstrap. It allows users to add, edit, delete, filter, and sort products, with data saved using localStorage.

🔧 Features
Product Fields
Product ID (Auto-generated)

Product Name

Product Image

Price

Description

Core Functions
Add Product – Form with real-time validation

Edit Product – Update details using URL query params

Delete Product – With confirmation and success popup

View Products – Displayed in card layout

Filter Products – By ID, Name, Price, or Description

Sort Products – By ID, Name, Price, or Description (asc/desc)

Responsive UI – Bootstrap layout with 2-column design

Persistent Storage – All data stored in localStorage

Dynamic Filter Feedback – Displays specific messages like “No products found for Product ID ‘17427230’.” when filters return no results

Image Size Restriction – Validates image uploads and restricts them to a maximum file size of 1MB, with a user-friendly alert: “Image file size should not exceed 1MB.”

✅ Validation Rules
Field Rules
Name Required, min 2 characters
Image Upload Required for new products, valid image formats only (JPG/PNG), max 1MB
Price Must be a number greater than 0
Description Required, min 10 characters
Real-Time Fields validate instantly as the user types
📦 How to Use
Click "Add Product" to create a new entry.

Use the Edit button to update product info.

Click Delete to remove a product (with confirmation).

Use Filter inputs to search specific products.

Use Sort dropdowns to organize products.

If no results are found, a clear message is shown.

Data is saved in localStorage and persists between sessions.

📁 Modular Code Structure
All core logic is organized into clean, maintainable TypeScript modules inside the src/ folder:

File Purpose
types.ts Shared type definitions (e.g., Product interface)
storage.ts Handles loading and saving products from localStorage
modal.ts Displays success confirmation popups using Bootstrap modals
product-form.ts Manages form input, validation, and saving new or edited products
product-list.ts Renders product cards, applies filters/sorting, and handles deletions
Each module handles a specific responsibility to keep the code clean, reusable, and easy to maintain.

💡 Tech Stack
HTML5

CSS3

Bootstrap 4

TypeScript (modular)

JavaScript (ES6 features)

LocalStorage API

Let me know if you want to add screenshots, a file tree, or deployment instructions next!

You said:
hey my above code is in typescript so change accordingly

ChatGPT said:
Ah, perfect — since your project is written in TypeScript, let's update the README.md to clearly reflect that.

Here’s your updated and well-structured README with TypeScript-specific terminology and refinements:

🛍️ Product Management System
A simple web-based Product Management System built with HTML, CSS, TypeScript, and Bootstrap. It allows users to add, edit, delete, filter, and sort products, with data stored in localStorage for persistence.

🔧 Features
Product Fields
Product ID (Auto-generated)

Product Name

Product Image

Price

Description

Core Functions
Add Product – Form with real-time validation and TypeScript enforcement

Edit Product – Update product details using query parameters

Delete Product – Includes a confirmation modal and success feedback

View Products – Displayed as responsive cards with clean Bootstrap layout

Filter Products – By ID, Name, Description, or Price

Sort Products – By ID, Name, or Price in ascending/descending order

Persistent Storage – All data is saved in localStorage

Responsive UI – Built with Bootstrap 4

Dynamic Filter Feedback – Displays specific messages like “No products found for Product ID ‘17427230’.” when filters return no results

Image Size Restriction – Image uploads are limited to 1MB, with a clear alert: “Image file size should not exceed 1MB.”

✅ Validation Rules
Field Rules
Name Required, minimum 2 characters
Image Upload Required for new products, JPG/PNG only, max 1MB
Price Must be a number greater than 0
Description Required, minimum 10 characters
Real-Time Fields validate instantly as the user types
📦 How to Use
Click "Add Product" to create a new entry.

Use the Edit button to update product info via query parameters.

Click Delete to remove a product (with confirmation modal).

Use Filter inputs to search for products by criteria.

Use Sort dropdowns to sort products by ID, name, or price.

When no results match the filters, a specific message is displayed.

All product data is saved in localStorage and persists across sessions.

📁 Modular TypeScript Structure
All business logic is written in TypeScript and modularized inside the src/ folder for better maintainability:

File Purpose
types.ts Shared TypeScript type definitions (e.g., Product interface)
storage.ts Handles loading and saving products from localStorage
modal.ts Displays success confirmation popups using Bootstrap modals
product-form.ts Manages form input, validation, and saving new or edited products
product-list.ts Renders product cards, applies filters/sorting, and handles deletions
Each module is responsible for a distinct feature, ensuring clean separation of concerns and type safety throughout the app.

💡 Tech Stack
HTML5

CSS3

TypeScript

Bootstrap 4

DOM APIs

LocalStorage API
