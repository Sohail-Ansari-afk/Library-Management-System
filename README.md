# 📚 Library Management System

A lightweight **Library Management System** built using **Python**, **Tkinter GUI**, and **SQLite database**. Easily manage books, issue and return them, track overdue returns, and more — all from a clean desktop interface. 🎯

---

## ✨ Features

- ➕ Add new books to the inventory
- 🔍 Search and view books by title
- 📦 Show all inventory or currently issued books
- 📤 Issue books to users
- 📥 Return books with automated late fee calculation
- ❌ Delete books (only if available)
- ⚠️ Input validation and user-friendly error messages

---

## 🛠️ Technologies Used

- 🐍 Python 3.x
- 🧰 Tkinter (for GUI)
- 🗃️ SQLite (for local database storage)
- 🧮 Custom fee calculator with date difference logic

---

## 📁 Project Structure

```

library-management/
├── main.py             # Entry point for GUI
├── ui.py               # Tkinter UI logic
├── database.py         # DB schema setup and connector
├── utils.py            # Fee calculation logic
├── library.db          # SQLite DB (auto-created if missing)

````

---

## 🚀 Getting Started

### ✅ Prerequisites

- Python 3.7 or above installed on your system  
- No external dependencies required!

### 📥 Installation

1. **Clone or Download this Repository**  
   ```bash
   git clone https://github.com/yourusername/library-management.git
   cd library-management
````

2. **Run the Application**

   ```bash
   python main.py
   ```

   > This will open a desktop window powered by Tkinter.

---

## 🧪 How to Use

### 🆕 Add a Book

* Fill in the **Title** and **Author**
* Click **"Add Book"**

### 📖 Show Inventory

* Click **"Show Inventory"**
* View available and issued books in the list

### 📤 Issue a Book

* Provide **Book ID** and **User Name**
* Click **"Issue Book"**
* System updates status to “Issued”

### 📥 Return a Book

* Provide **Issue ID** and optional **Return Date**
* Click **"Return Book"**
* System calculates and displays late fee (if any)

### 🔍 Search for a Book

* Enter partial/full title in **Search Title**
* Click **"Search Book"** to view matching results

### ❌ Delete a Book

* Enter **Book ID** (must not be issued)
* Click **"Delete Book"**

---

## 📊 Late Fee Calculation

* First 14 days: **Free**
* After 14 days: **₹2/day**
* Auto-calculated using return vs issue date via:

  ```python
  (return_date - issue_date).days
  ```

---

## 📌 Notes

* The database `library.db` is created automatically.
* You can reset the app by deleting this file and restarting.
* Ensure valid input format for dates: `YYYY-MM-DD`

---

## 👨‍💻 Author

Made with ❤️ by SOhail-Ansari

---

## 🧾 License

This project is licensed under the MIT License.
Feel free to fork and modify!

``

Happy coding! 😄📚
```
