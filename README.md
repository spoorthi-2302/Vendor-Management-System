Project name:
Vendor management system

Objective:
A Vendor Management System using Django and Django REST Framework. This system will handle vendor profiles, track purchase orders, and calculate vendor performance metrics.

Table of Contents
Getting started
Prequisites
Installation
API Endpoints
Contributing
License
Acknowledgments

Prequisites:
- Python (version 3.11.2)
- Django (version 4.1.2)
- Django Rest Framework (version 3.14.0)

Installation:
1. Clone the repository

2. Install dependencies:
pip install django
pip install djangorestframework

3. Apply database migrations:
make sure you are inside vms directory inside inventory.
cd vms
python manage.py makemigrations
python manage.py migrate

4. Create a superuser account (for admin access):
python manage.py createsuperuser

5. Start the development server:
python manage.py runserver

6. Access the Django admin interface at `http://127.0.0.1:8000/admin/` and log in with the superuser credentials.

API Endpoints:
Vendors

List and Create Vendors
  - Endpoint: /vendors/
  - Method: GET (List all vendors), POST (Create a new vendor)
  - Example: http://localhost:8000/vendors/

Retrieve, Update, and Delete Vendor:
  - Endpoint: vendors/<vendor_id>/
  - Methods: GET (Retrieve), PUT (Update), DELETE (Delete)
  - Example:  http://localhost:8000/vendors/1/

Purchase Orders

List and Create Purchase Orders:
  - Endpoint: /purchase-orders/
  - Method: GET (List all purchase orders), POST (Create a new purchase order)
  - Example: http://localhost:8000/purchase-orders/

Retrieve, Update, and Delete Purchase Order:**
  - Endpoint: /purchase-orders/<purchase_order_id>/
  - Methods: GET (Retrieve), PUT (Update), DELETE (Delete)
  - Example:http://localhost:8000/api/purchase-orders/1/

Vendor Performance Metrics

Retrieve Vendor Performance Metrics:
  - Endpoint: vendors/<vendor_id>/performance/
  - Method: GET
  - Example: http://localhost:8000/api/vendors/1/performance/`

