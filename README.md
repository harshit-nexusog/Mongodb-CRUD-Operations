
# MongoDB CRUD Operations

This project demonstrates the basic **CRUD (Create, Read, Update, Delete)** operations in MongoDB using Python.

It is designed as a beginner-friendly project to understand how Python applications interact with a MongoDB database.

## 📌 Features

* Create new records
* Read and display records
* Update existing records
* Delete records
* Connect Python with MongoDB
* Perform database operations using MongoDB queries

## 🛠️ Technologies Used

* **Python**
* **MongoDB**
* **PyMongo**
* **MongoDB Compass** (optional)
* **VS Code**

## 📂 CRUD Operations

### 1. Create

Adds a new document to the MongoDB collection.

```python
collection.insert_one({
    "name": "Harshit",
    "course": "BCA",
    "age": 20
})
```

### 2. Read

Retrieves documents from the MongoDB collection.

```python
for student in collection.find():
    print(student)
```

### 3. Update

Updates information in an existing document.

```python
collection.update_one(
    {"name": "Harshit"},
    {"$set": {"age": 21}}
)
```

### 4. Delete

Deletes a document from the collection.

```python
collection.delete_one({"name": "Harshit"})
```

## 📁 Project Structure

```text
MongoDB-CRUD/
│
├─file
report on crud operations

## ⚙️ Installation

### Step 1: Install Python

Make sure Python is installed on your system.

### Step 2: Install PyMongo

Open the terminal and run:

```bash
pip install pymongo
```

### Step 3: Install MongoDB

Install MongoDB Community Server or use MongoDB Atlas.

### Step 4: Connect MongoDB

Example connection:

```python
from pymongo import MongoClient

client = MongoClient("mongodb://localhost:27017/")
db = client["student_db"]
collection = db["students"]
```

## ▶️ How to Run

Clone the repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_LINK
```

Open the project folder:

```bash
cd MongoDB-CRUD
```

Run the Python file:

```bash
python crud.py
```

## 📊 Example Data

| Name    | Course | Age |
| ------- | ------ | --: |
| Harshit | BCA    |  20 |
| Rahul   | BCA    |  21 |
| Gauri   | BCA    |  20 |

## 🎯 Learning Objectives

Through this project, you can learn:

* MongoDB database basics
* Collections and documents
* CRUD operations
* MongoDB queries
* Python-MongoDB connectivity
* Basic database management

## 🔮 Future Improvements

* Add a graphical user interface
* Add search functionality
* Add input validation
* Add more database collections
* Convert it into a complete Student Management System

## 👨‍💻 Author

**Harshit Srivastava**

BCA (Data Science & Artificial Intelligence)



This project is created for **educational and learning purposes**.
