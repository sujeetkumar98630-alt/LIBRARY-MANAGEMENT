# Library Management System

A modular, command-line Library Management System built with Python. This project allows users to manage a simple book inventory with core functionalities to add, issue, return, and display books.

## Features

* **Add Books:** Easily add new book titles to the library inventory.
* **Issue Books:** Assign available books to users. The system handles multiple copies of the same title and includes a 15-day return policy reminder.
* **Return Books:** Process returning books, automatically moving them from the issued list back into the available inventory.
* **View Inventory:** Display all currently available books in the library.
* **Dynamic Indexing:** Automatically renumbers book IDs to maintain a clean, sequential list after any inventory modifications.

## Project Structure

The application logic is separated into specific modules for better maintainability and organization:

| File | Description |
| :--- | :--- |
| **`main.py`** | The main entry point of the program. Contains the interactive menu loop. |
| **`add_book.py`** | Handles capturing user input and adding new book records to the database. |
| **`issue_book.py`** | Manages searching for available books, handling multiple copies, and moving books to the issued list. |
| **`return_book.py`** | Validates returning books and restores them to the main library collection. |
| **`show_book.py`** | Neatly displays the current available books in a numbered list. |
| **`utils.py`** | Acts as the central data storage (dictionaries) and holds helper functions like `renumber_books()`. |
