# GoDataHub API

## 📌 Project Overview

This project is a simple **CRUD API** built using **Golang** and **MongoDB**. It allows users to perform **Create, Read, Update, and Delete (CRUD)** operations on a MongoDB database via RESTful API endpoints.

## 🚀 Features

- Create a new record
- Retrieve all records
- Retrieve a single record by ID
- Update an existing record
- Delete a record

## 🛠️ Tech Stack

- **Programming Language:** Go (Golang)
- **Database:** MongoDB
- **Framework:** Gin (for routing)
- **Driver:** go.mongodb.org/mongo-driver

## 📂 Project Structure

```
├── main.go
├── config/
│   ├── database.go
├── models/
│   ├── item.go
├── routes/
│   ├── routes.go
├── controllers/
│   ├── itemController.go
├── go.mod
├── go.sum
├── .env
└── README.md
```

## 📌 Prerequisites

Make sure you have the following installed:

- [Golang](https://golang.org/dl/)
- [MongoDB](https://www.mongodb.com/try/download/community)
- [Postman](https://www.postman.com/) (for testing API requests)

## 🔧 Installation & Setup

1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/go-mongo-crud.git
   cd go-mongo-crud
   ```
2. Install dependencies:
   ```sh
   go mod tidy
   ```
3. Configure environment variables:
   Create a `.env` file and add:
   ```env
   MONGO_URI=mongodb://localhost:27017
   DATABASE_NAME=mydatabase
   COLLECTION_NAME=items
   ```
4. Run the project:
   ```sh
   go run main.go
   ```

## 📡 API Endpoints

| Method | Endpoint      | Description       |
| ------ | ------------- | ----------------- |
| GET    | `/items`      | Get all items     |
| GET    | `/items/{id}` | Get item by ID    |
| POST   | `/items`      | Create new item   |
| PUT    | `/items/{id}` | Update item by ID |
| DELETE | `/items/{id}` | Delete item by ID |

## 🛠 Sample Request (Postman)

### Create Item (POST)

```json
{
  "name": "Laptop",
  "price": 1200,
  "category": "Electronics"
}
```

## 📜 License

This project is licensed under the MIT License.

## 👨‍💻 Author

- **Your Name** – [GitHub Profile](https://github.com/anandku06)
