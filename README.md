# GemCart Backend API

Flask-based REST API for GemCart e-commerce platform.

## Features
- User authentication (JWT)
- Product CRUD operations
- Order management
- Category management
- Search functionality

## Tech Stack
- Flask
- SQLAlchemy
- Flask-JWT-Extended
- SQLite

## Setup

```bash
pip install -r requirements.txt
python app.py
```

**API URL:** http://localhost:5000

## API Endpoints

### Auth
- `POST /api/auth/register` - Register user
- `POST /api/auth/login` - Login user

### Products
- `GET /api/products/` - Get all products
- `GET /api/products/<id>` - Get single product
- `POST /api/products/` - Create product (sellers only)
- `PUT /api/products/<id>` - Update product
- `DELETE /api/products/<id>` - Delete product

### Orders
- `POST /api/orders/` - Create order
- `GET /api/orders/` - Get user orders

### Categories
- `GET /api/categories/` - Get all categories

### Search
- `GET /api/search?q=query` - Search products

## Test Account
- Email: seller@gemcart.com
- Password: password