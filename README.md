# Business Inventory Management System (BIMS)

## **Overview**
The Business Inventory Management System (BIMS) is a robust web application designed to streamline inventory tracking, customer management, and sales order processing. Developed using the Flask framework, this project is ideal for small-to-medium businesses looking for a scalable and secure inventory solution.

---

## **Features**

1. **Inventory Management**
   - Add, edit, and delete product information.
   - Track stock levels and receive low-stock alerts.

2. **Customer Management**
   - Maintain a database of customer details.
   - Search and filter customers easily.

3. **Sales Orders**
   - Create, view, and manage sales orders.
   - Generate sales summaries and analytics.

4. **User Authentication**
   - Role-based access control (Admin and Staff).
   - Secure login/logout functionality.

5. **APIs**
   - Consume external APIs for dynamic functionality (e.g., currency conversion).
   - Expose internal APIs for integration.

6. **Deployment**
   - Production-ready deployment with security measures.
   - Hosted on platforms like AWS or Heroku.

---

## **Technology Stack**

- **Backend Framework:** Flask (Python)
- **Database:** SQLite (development), PostgreSQL (production)
- **Frontend:** HTML, CSS (Bootstrap), Jinja2 Templates
- **Authentication:** Flask-Login
- **API Development:** Flask-RESTful
- **Deployment:** Gunicorn, Nginx, Heroku/AWS

---

## **Installation Instructions**

### **Prerequisites**
- Python 3.8+
- Virtual Environment (optional but recommended)

### **Steps**
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/barasamichael/Web-Development-Course-Code-Base.git
   cd Web-Development-Course-Code-Base
   ```

2. **Create a Virtual Environment:**
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up the Database:**
   ```bash
   flask db init
   flask db migrate
   flask db upgrade
   ```

5. **Run the Development Server:**
   ```bash
   flask run
   ```
   Access the application at `http://127.0.0.1:5000`.

---

## **Usage Guide**

1. **Admin Setup:**
   - Create an admin user using the Flask CLI or database seeding.

2. **Add Products:**
   - Navigate to the inventory page and add products.

3. **Manage Customers:**
   - Add or edit customer details through the customer management interface.

4. **Process Orders:**
   - Use the sales orders feature to create and track orders.

5. **Low-Stock Alerts:**
   - Monitor stock levels to ensure timely restocking.

---

## **API Endpoints**

| Method | Endpoint                 | Description                       |
|--------|--------------------------|-----------------------------------|
| GET    | `/api/products`          | Retrieve all products.            |
| POST   | `/api/products`          | Add a new product.                |
| GET    | `/api/customers`         | Retrieve all customers.           |
| POST   | `/api/orders`            | Create a new sales order.         |
| GET    | `/api/orders/<order_id>` | Retrieve details of a sales order.|

---

## **Contributing**

1. Fork the repository and clone it locally.
2. Create a new branch for your feature:
   ```bash
   git checkout -b feature-name
   ```
3. Commit and push your changes:
   ```bash
   git commit -m "Description of changes"
   git push origin feature-name
   ```
4. Create a pull request.

---

## **License**
None

---

## **Contact**
For inquiries or support, contact:
- **Email:** michael.barasa@strathmore.edu
- **GitHub Issues:** [Issues Page](https://github.com/barasamichael/Web-Development-Course-Code-Base/issues)
