# Shopy

Shopy is a multi-user e-commerce application built with Laravel.  
It is designed as an educational project that demonstrates how to build a complete online store with multiple user roles, dashboards, order management, and online payments.

The system supports **admins**, **merchants**, and **customers**, each with their own permissions and workflows.  
It combines traditional Blade dashboards with modern **Filament admin panels**, along with a RESTful API for core e-commerce operations.

---

## 🚀 Features

### General
- Multi-user e-commerce system
- Authentication and authorization
- Role-based access control (Admin, Merchant, Customer)
- RESTful API architecture
- File and image upload handling
- Clean API responses using Resources and Helpers

### Admin Features
- Admin authentication
- Manage categories
- Manage merchants and customers
- Manage products
- View and manage orders
- Filament-based admin panel
- Artisan command to create admin users

### Merchant Features
- Merchant registration and authentication
- Product management (CRUD)
- Product image management
- Manage received orders
- Update order item status
- Merchant-specific API resources and policies

### Customer Features
- Customer authentication
- Browse products and categories
- Shopping cart system
- Add, update, and remove cart items
- Checkout process
- Shipping address management
- Order creation and order status tracking
- Stripe payment integration

### Orders & Payments
- Order and order item management
- Order status tracking
- Stripe payment gateway integration
- Payment records stored in the database

### System & Architecture
- Blade-based dashboards
- Filament admin resources
- Middleware for role checking
- Policies for authorization
- Observers for automatic model handling
- Jobs for background processing
- Custom validation rules
- Service-based authentication logic

---

## 🛠 Tech Stack

- **Language:** PHP
- **Framework:** Laravel
- **Database:** MySQL
- **Frontend (Dashboards):**
  - Blade
  - Filament
- **Payment Gateway:** Stripe
- **Architecture:** MVC + Service-based structure

---

## 📂 Project Structure Overview

- `Controllers` – Handle API and web requests
- `Filament` – Admin panel resources
- `Models` – Application data models
- `Requests` – Request validation
- `Resources` – API response formatting
- `Middleware` – Role and access control
- `Policies` – Authorization logic
- `Observers` – Model lifecycle handling
- `Jobs` – Background tasks
- `Services` – Business logic
- `Traits` – Shared model functionality
- `Helpers` – Response formatting utilities

---

## ⚙️ Installation & Setup

### Prerequisites
- PHP >= 8.1
- Composer
- MySQL
- Stripe account (for payments)

### Steps

```bash
git clone https://github.com/RanaAbuarabDev/shopy.git
cd shopy
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
php artisan serve
