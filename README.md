# 🍽️ Foodies API - Backend for Food Delivery App

This is the backend service for the **Foodies App**, developed using **Spring Boot** and **MySQL**, with **Razorpay** integrated for payment processing. This project handles user registration, authentication, food listings, cart management, order placement, and payment verification.

---

## 📌 API Endpoints

### 🧾 Food Management
| Method | Endpoint       | Description          |
|--------|----------------|----------------------|
| POST   | /addFood       | Add a new food item  |
| GET    | /foods         | Get list of foods    |
| GET    | /food/{id}     | Get food by ID       |
| DELETE | /food/{id}     | Delete a food item   |

### 👤 User Authentication
| Method | Endpoint     | Description         |
|--------|--------------|---------------------|
| POST   | /register    | Register a user     |
| POST   | /login       | User login          |

### 🛒 Cart Management
| Method | Endpoint         | Description                  |
|--------|------------------|------------------------------|
| POST   | /cart/add        | Add item to cart             |
| GET    | /cart            | Get cart items               |
| DELETE | /cart/clear      | Clear entire cart            |
| POST   | /cart/remove     | Remove specific item         |

### 📦 Order & Payment
| Method | Endpoint             | Description                   |
|--------|----------------------|-------------------------------|
| POST   | /order/create        | Create a new order            |
| POST   | /payment/verify      | Verify Razorpay payment       |
| GET    | /orders              | Get orders of logged-in user  |
| GET    | /orders/all          | Get all orders (Admin only)   |
| PATCH  | /order/status/{id}   | Update order status           |
| DELETE | /order/{id}          | Remove an order               |

---

## 🛠️ Technologies Used

- Java 21
- Spring Boot
- Spring Security (JWT-based)
- MySQL
- Maven
- Razorpay Payment Gateway

---

## 🧪 Testing Payment

A sample `checkout.html` page is provided to test Razorpay integration.  
To use it:
1. Replace the Razorpay key in the script.
2. Open the HTML file in a browser.
3. Make a test payment.

---

## 🚀 Running the Project

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/foodies-api.git
   cd foodies-api
