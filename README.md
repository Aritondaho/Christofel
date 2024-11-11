
Christofel Menu App
The Christofel Menu App is a mobile application developed using React Native. It helps restaurant owners or users to manage and display their menu items with details like name, price, and type (Main Course, Dessert, etc.). The app also allows users to filter the menu by course type, calculate average prices for each type, and add new menu items dynamically.

Features
View Menu: Displays menu items categorized by their type (Main Course, Dessert, etc.).
Add Menu Item: A form to add new items to the menu.
Filter Menu: Filters menu items by course type (Main Course, Dessert, All Items).
Average Price Calculation: Displays average prices for each course type.
Dynamic Menu Updates: Menu is updated in real-time when items are added or filtered.
Improvements and Updates
1. Efficient State Management
Custom Hook (useMenuItems):
Manages the menuItems state in a more modular and reusable way.
Provides functions like addMenuItem, filterMenuItems, and getAveragePriceByType to manage menu data.
Keeps the UI code clean and readable by separating logic from rendering.
2. Menu Grouping by Course Type
Menu items are now grouped by their type (e.g., Main Course, Dessert).
Each group of menu items has its own section with the average price displayed.
Users can see the menu items categorized automatically, improving readability and organization.
3. Filtering and Sorting
Filters allow users to see only specific categories (Main Course, Dessert) or all items.
Average price is calculated dynamically for each course type, which helps with menu analysis and user experience.
4. UI/UX Enhancements
Improved UI Components: The app uses reusable components for each menu item.
Seamless Navigation: Clear navigation between screens using React Navigation.
FlatList: Efficient rendering of menu items using FlatList to handle potentially large datasets.
5. Image Mapping
Each menu item has an associated image. Users can see pictures along with the names and prices.
Images are mapped using item names to ensure that each menu item has an appropriate image.
6. Bug Fixes
State Management Fixes: Resolved issues where setMenuItems was undefined or not passed correctly to child components.
Filtering Logic: Fixed issues where filtering the menu wasn't updating the state correctly.
Project Structure
The project follows a modular and scalable structure:

bash
Copy code
/assets                # Store images used for the menu items
/components            # Reusable components (e.g., MenuItem.js)
/Screens               # Screen components (e.g., HomeScreen.js, AddMenuItemScreen.js)
/hooks                 # Custom hooks (e.g., useMenuItems.js)
/App.js                # Entry point for the app
Key Components:
HomeScreen.js: Displays the list of menu items, grouped by course type, and includes buttons for filtering and adding items.
AddMenuItemScreen.js: A screen to add new items to the menu, including fields for item name, price, and course type.
MenuItem.js: A reusable component for rendering individual menu items.
FilterMenuScreen.js: A screen that allows users to filter menu items based on their course type
