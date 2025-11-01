🌸 AgriSmart API

Developed by Phillip & Phoebe

AgriSmart API is a simple Express.js project that manages flower products with authentication, middleware, and filtering features.

🚀 Features

RESTful CRUD API for products

Custom middleware (logger, authentication)

Error handling for stability

Advanced features: filtering, pagination, and search

🧰 Setup

Clone the repository

git clone <repo-url>
cd agrismart-api


Install dependencies

npm install


Run the server

npm start


Test the API
Use Postman, Insomnia, or curl to test the endpoints.

🧩 API Endpoints
Method	Endpoint	Description
GET	/api/products	Get all products
GET	/api/products/:id	Get single product
POST	/api/products	Create a new product
PUT	/api/products/:id	Update a product
DELETE	/api/products/:id	Delete a product
🔐 Authentication

All product routes require an Authorization header:

Authorization: secret123


If missing or incorrect, the server responds with 403 Unauthorized.

🔍 Example Request
POST /api/products
Headers: { "Authorization": "secret123" }
Body: { "name": "Lilies", "price": 250 }

Example Response
{
  "id": 3,
  "name": "Lilies",
  "price": 250
}

⚙️ Filtering, Pagination, Search

You can query products with:

/api/products?name=rose&minPrice=100&maxPrice=300&page=1&limit=5

🧑‍💻 Developers

Phillip & Phoebe
Creators and developers of AgriSmart — a platform connecting flower farmers to markets.

© 2025 AgriSmart — Built with ❤️ using Express.js 🌿
