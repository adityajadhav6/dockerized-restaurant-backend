# 🍽️ Restaurant Management System Backend

Welcome to the **Restaurant Management System Backend**! This project is a Node.js-based backend application designed to manage restaurant tables, orders, and statuses efficiently. 🚀

---

## 🌟 Features
- 🛠️ **CRUD Operations** for managing tables and orders.
- 🗄️ **MongoDB Integration** for seamless data storage.
- 🐳 **Dockerized Setup** for easy deployment and scalability.
- 🔐 **Environment Configuration** using `.env` files.

---

## 📂 Project Structure
```plaintext
server/
├── models/          # Mongoose schemas
├── routes/          # API routes
├── [.env.example]   # Environment variable template
├── Dockerfile       # Docker configuration
├── [docker-compose.yml] # Docker Compose setup
└── [server.js]      # Main server file
```

## Prerequisites


- Node.js (v18 or higher)
- Docker
- MongoDB (local or cloud-based)

## 🛠️ Installation
1. Clone the Repository:
```plaintext
git clone <repository-url>
cd restaurant-management-system/server
```

2. Install Dependencies:
```plaintext
npm install
```

3. Set up Environment Variables:
```plaintext
cp .env.example .env
```
4. Run Locally:
```plaintext
npm run dev
```
The server will start at http://localhost:5001

## 🐳 Running with Docker
1. Build and Start Containers:

```plaintext
docker-compose up --build
```
2. Access the Backend:
  -  API: http://localhost:5001
  - MongoDB: mongodb://mongo:27017/restaurant

3. Stop Containers:
   ```plaintext
   docker-compose down
   ```
## 📖 API Endpoints
Use Postman for making the API calls.
 - GET /api/tables : Fetch all tables.
- GET /api/tables/name/:name : Fetch a table by name.
- POST /api/tables : Create a new table.
- PATCH /api/tables/:id/orders : Add an order to a table.
- DELETE /api/tables/:id : Delete a table by ID.

   ## 🛠️ Built With
- Node.js - Backend runtime.
- Express.js - Web framework.
- MongoDB - Database.
- Mongoose - ODM for MongoDB.
- Docker - Containerization.

  ## 🤝 Contributing
  Contributions are welcome! Feel free to Fork the repository and submit a pull request.

  ## 🎉 Happy Coding!
