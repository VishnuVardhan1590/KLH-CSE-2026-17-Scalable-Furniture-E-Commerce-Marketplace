# Scalable Furniture E-Commerce Marketplace

## Team Members

| Name                | ID Number  |
| -------------       | ---------- |
| I. Vishnu Vardhan   | 2420030513 |
| S. Roshan Sai       | 2420030522 |
| M. Pranay Sai Varma | 2420030756 |
| A. Srinivas         | 2420030559 |

## Supervisor

**Supervisor Name:** RajKumar Patil

---

## Abstract

The **Scalable Furniture E-Commerce Marketplace** is an online platform designed to provide customers with a convenient and user-friendly way to browse, search, compare, and purchase furniture products online.

The platform provides a centralized marketplace where furniture products can be displayed with detailed information such as product name, category, price, description, images, and availability. Customers can explore different furniture products, add items to their shopping cart, and manage their purchases through an easy-to-use interface.

The system is designed with scalability and maintainability in mind so that additional products, users, features, and services can be integrated as the platform grows.

---

## Project Description

The **Scalable Furniture E-Commerce Marketplace** is a web-based e-commerce application developed to simplify the process of buying and selling furniture online.

The platform allows customers to explore different categories of furniture such as sofas, chairs, tables, beds, wardrobes, cabinets, and other home and office furniture.

The system provides essential e-commerce functionalities including product browsing, product search, product filtering, product details, shopping cart management, user authentication, and order management.

The marketplace architecture is designed to support future expansion, allowing new product categories, payment systems, recommendation systems, seller accounts, and other e-commerce services to be integrated.

---

## Objectives

* Develop a scalable online marketplace for furniture products.
* Provide an easy-to-use interface for customers.
* Allow users to browse and search for furniture products.
* Provide detailed information about furniture products.
* Implement product categorization and filtering.
* Allow customers to add products to a shopping cart.
* Implement user registration and authentication.
* Provide order management functionality.
* Maintain product and customer information efficiently.
* Design the system for future scalability and feature expansion.
* Provide a reliable and responsive e-commerce experience.

---

## Key Features

### Customer Features

* User registration and login
* Browse furniture products
* Search products
* Product categories
* Product filtering and sorting
* Product details
* Add products to cart
* Update cart quantity
* Remove products from cart
* Order placement
* Order history
* User profile management

### Marketplace Features

* Furniture product management
* Product categorization
* Product inventory management
* Product pricing
* Product availability tracking
* Order management
* Customer management

### Future Features

* Online payment integration
* Seller/vendor management
* Product reviews and ratings
* Wishlist
* Personalized product recommendations
* AI-based furniture recommendations
* Delivery tracking
* Discount and coupon management
* Analytics dashboard

---

## Technology Stack

* **Frontend:** HTML, CSS, JavaScript
* **Backend:** Python
* **Framework:** Flask / FastAPI
* **Database:** MySQL / SQLite
* **Data Processing:** Python
* **API:** REST API
* **Version Control:** Git
* **Repository:** GitHub

> Update the backend framework and database names according to the technologies actually used in your project.

---

## System Architecture

The system follows a modular architecture consisting of the following major components:

```text
                    ┌─────────────────────┐
                    │      Customer       │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Frontend / UI     │
                    │ HTML/CSS/JavaScript │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    Backend API      │
                    │  Python Framework   │
                    └──────────┬──────────┘
                               │
              ┌────────────────┼────────────────┐
              │                │                │
              ▼                ▼                ▼
       ┌────────────┐   ┌────────────┐   ┌────────────┐
       │  Products  │   │   Users    │   │   Orders   │
       └────────────┘   └────────────┘   └────────────┘
              │                │                │
              └────────────────┼────────────────┘
                               ▼
                    ┌─────────────────────┐
                    │      Database       │
                    └─────────────────────┘
```

---

## Project Structure

```text
Scalable-Furniture-E-Commerce-Marketplace/
│
├── README.md
│
├── frontend/
│   ├── index.html
│   ├── products.html
│   ├── product-details.html
│   ├── cart.html
│   ├── login.html
│   ├── register.html
│   └── css/
│       └── style.css
│
├── backend/
│   ├── app.py
│   ├── routes/
│   ├── models/
│   ├── services/
│   └── config.py
│
├── database/
│   ├── schema.sql
│   └── database.db
│
├── static/
│   ├── images/
│   └── assets/
│
├── templates/
│   └── ...
│
├── requirements.txt
└── .gitignore
```

> The project structure may be updated as development progresses.

---

## Main Modules

### 1. User Management

The user management module handles:

* User registration
* User login
* Authentication
* User profile information
* Account management

### 2. Product Management

The product management module handles furniture products including:

* Product name
* Product description
* Product category
* Product price
* Product images
* Product availability
* Product inventory

### 3. Search and Filter

Customers can search for furniture products and filter products based on:

* Category
* Price
* Product type
* Availability
* Other relevant attributes

### 4. Shopping Cart

The shopping cart module allows customers to:

* Add products
* Remove products
* Change quantities
* View total price
* Review selected products before checkout

### 5. Order Management

The order management module handles:

* Order creation
* Order details
* Customer information
* Product information
* Order status
* Order history

### 6. Database Management

The database stores and manages:

* User information
* Product information
* Categories
* Cart information
* Order information
* Inventory information

---

## Setup and Execution Instructions

### 1. Clone the Repository

```bash
git clone <repository-url>
```

### 2. Navigate to the Project Directory

```bash
cd Scalable-Furniture-E-Commerce-Marketplace
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

### 4. Activate the Virtual Environment

**Windows:**

```bash
venv\Scripts\activate
```

**Linux/macOS:**

```bash
source venv/bin/activate
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

### 6. Run the Application

If using Flask:

```bash
python backend/app.py
```

If using FastAPI:

```bash
uvicorn backend.app:app --reload
```

### 7. Open the Application

For a Flask application, the local URL is typically:

```text
http://127.0.0.1:5000
```

For a FastAPI application, the local URL is typically:

```text
http://127.0.0.1:8000
```

---

## Database

The application uses a database to store and manage marketplace information.

The major database entities include:

```text
Users
  │
  ├── User ID
  ├── Name
  ├── Email
  └── Password

Products
  │
  ├── Product ID
  ├── Product Name
  ├── Category
  ├── Price
  ├── Description
  └── Stock

Cart
  │
  ├── Cart ID
  ├── User ID
  ├── Product ID
  └── Quantity

Orders
  │
  ├── Order ID
  ├── User ID
  ├── Product ID
  ├── Quantity
  ├── Total Amount
  └── Order Status
```

---

## Scalability

The platform is designed with scalability as a major consideration.

The system can be extended to support:

* Large product catalogs
* Multiple sellers
* Increasing numbers of customers
* Distributed database systems
* Cloud deployment
* RESTful APIs
* Microservices architecture
* Caching
* Load balancing
* Cloud-based storage
* Product recommendation systems

The modular design makes it easier to add new features without significantly affecting existing functionality.

---

## Security

The application aims to provide basic security mechanisms including:

* User authentication
* Password protection
* Input validation
* Secure API endpoints
* Database access control
* Session management
* Protection against unauthorized access

Additional security mechanisms can be integrated during future development.

---

## Current Phase Status

### Phase 1 – Project Planning

**Status: Completed ✅**

* Project idea finalized
* Problem statement identified
* Project objectives defined
* E-commerce requirements identified
* Technology stack planned

### Phase 2 – System Design

**Status: In Progress 🔄**

* System architecture being designed
* Database structure being planned
* Product management workflow designed
* Shopping cart workflow planned
* User interface design in progress

### Phase 3 – Implementation

**Status: In Progress 🔄**

* Frontend development
* Backend development
* Database integration
* Product management
* User authentication
* Shopping cart implementation
* Order management

### Phase 4 – Testing and Deployment

**Status: Not Started ⏳**

* Functional testing
* Database testing
* API testing
* Security testing
* Performance testing
* Deployment

> Update the phase statuses according to the actual progress of your team.

---

## Future Enhancements

* Multi-vendor marketplace support
* Online payment gateway integration
* AI-powered furniture recommendations
* Augmented Reality (AR) furniture preview
* Product reviews and ratings
* Wishlist functionality
* Personalized recommendations
* Advanced product search
* Delivery tracking
* Inventory automation
* Discount and coupon system
* Customer support chatbot
* Cloud deployment
* Mobile application
* Analytics and reporting dashboard

---

## Applications

The Scalable Furniture E-Commerce Marketplace can be useful for:

* Furniture retailers
* Online furniture stores
* Home decor businesses
* Office furniture suppliers
* Furniture manufacturers
* Multi-vendor furniture marketplaces

---

## Advantages

* Easy online furniture shopping
* Centralized product marketplace
* Simple product discovery
* Reduced manual effort
* Scalable architecture
* Easy product management
* Convenient shopping cart and ordering
* Supports future AI and cloud integration
* User-friendly interface

---

## Project Goals

The primary goal of this project is to develop a **scalable, reliable, and user-friendly furniture e-commerce marketplace** that connects customers with furniture products through a modern digital platform.

The project focuses on creating a strong foundation that can be expanded in the future with advanced technologies such as **Artificial Intelligence, cloud computing, recommendation systems, AR visualization, and multi-vendor marketplace capabilities**.

---

## License

This project is developed for **academic purposes**.
