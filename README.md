# DRF Shop

DRF Shop is an e-commerce platform built using Django and Django REST Framework (DRF). This project provides APIs for managing products, orders, and users.

## Features

- User authentication and authorization
- Product listing and detail views
- Cart management
- Order creation and tracking
- Admin panel for managing products and orders

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/AlexTkDev/drf-shop.git
   cd drf-shop
   ```

2. Create and activate a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the migrations:
   ```bash
   python manage.py migrate
   ```

5. Create a superuser:
   ```bash
   python manage.py createsuperuser
   ```

6. Start the development server:
   ```bash
   python manage.py runserver
   ```

## Usage

### API Endpoints

#### Authentication

- **Register**: `POST /api/auth/register/`
- **Login**: `POST /api/auth/login/`
- **Logout**: `POST /api/auth/logout/`

#### Products

- **List products**: `GET /api/products/`
- **Product details**: `GET /api/products/<id>/`

#### Cart

- **View cart**: `GET /api/cart/`
- **Add to cart**: `POST /api/cart/add/`
- **Remove from cart**: `POST /api/cart/remove/`

#### Orders

- **Create order**: `POST /api/orders/create/`
- **Order details**: `GET /api/orders/<id>/`

### Admin Panel

To access the admin panel, go to `http://127.0.0.1:8000/admin/` and log in with the superuser credentials.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request.

## License

This project is licensed under the MIT License.
