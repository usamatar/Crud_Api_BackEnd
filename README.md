# Node.js API with MongoDB CRUD Operations

This project is a simple Node.js-based REST API for managing products, built using MongoDB for data storage. It includes endpoints for creating, reading, updating, and deleting products.

## Features
- Create, Read, Update, and Delete (CRUD) operations for products.
- MongoDB as the database.
- Modular structure with separate route and controller files.

## Requirements
Make sure you have the following installed:
- Node.js
- MongoDB

## Getting Started

### 1. Clone the Repository
```bash
git clone <repository-url>
cd <repository-folder>
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Set Up Environment Variables
Create a `.env` file in the root directory and configure the following variables:
```
PORT=3004
DB_URL=mongodb://localhost:27017/your-database-name
```

### 4. Start the Server
```bash
npm start
```
The server will run on the specified `PORT` (default is 3004).

### 5. Test the API
Use a tool like [Postman](https://www.postman.com/) or [Insomnia](https://insomnia.rest/) to interact with the API.

## API Endpoints

### Base URL
```
http://localhost:<PORT>/api/products
```

### Endpoints
| Method | Endpoint        | Description              |
|--------|-----------------|--------------------------|
| GET    | `/`             | Welcome message          |
| GET    | `/api/products` | Get all products         |
| GET    | `/api/products/:id` | Get a product by ID    |
| POST   | `/api/products` | Create a new product     |
| PUT    | `/api/products/:id` | Update a product by ID |
| DELETE | `/api/products/:id` | Delete a product by ID |

## Project Structure
```
project-folder/
├── controllers/
│   └── product.controller.js
├── models/
│   └── product.model.js
├── routes/
│   └── product.route.js
├── .env
├── app.js
└── package.json
```

### Explanation
- **controllers/**: Contains logic for handling API requests.
- **models/**: Defines the product schema for MongoDB.
- **routes/**: Contains route definitions for the product endpoints.
- **app.js**: Entry point of the application.
- **.env**: Environment variables.

## Contributing
Feel free to fork this repository and submit pull requests. Contributions are welcome!

## License
This project is licensed under the MIT License.

