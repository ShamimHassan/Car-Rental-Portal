🚗 Car Rental Management System

A complete PHP & MySQL-based Car Rental Management System designed for online vehicle booking and administrative management. This system allows users to search, view, and book vehicles, while the admin panel provides full control over vehicles, brands, bookings, testimonials, subscribers, and website content.

This project is suitable for Final Year Projects, portfolio showcase, and real-world deployment (cPanel ready).

📌 Project Description

- The Car Rental Management System is a dynamic web application that enables customers to:
  - Search available vehicles
  - View detailed car information
  - Book cars online
  - Manage their profile and bookings
- The Admin panel allows complete backend management including vehicle listing, brand management, booking confirmation, testimonials, contact queries, and subscribers.

🎯 Key Features

👤 User Features

- User Registration & Login
- Car Search & Filtering
- Vehicle Details View
- Online Booking System
- Booking History (My Booking)
- Profile Management
- Password Update
- Post Testimonials
- Contact Form

🔐 Admin Features

- Admin Dashboard with Statistics
- Manage Vehicles (Add/Edit/Delete)
- Manage Brands
- Manage Bookings (New, Confirmed, Cancelled)
- Manage Registered Users
- Manage Testimonials
- Manage Contact Queries
- Manage Pages (About, Contact etc.)
- Manage Subscribers
- Change Admin Password

🛠 Technologies Used

🌐 Frontend

- HTML5
- CSS3
- Bootstrap
- JavaScript
- jQuery
- DataTables
- Chart.js

⚙ Backend

- PHP (Core PHP)
- MySQL

🗄 Database

- MySQL Database (carrental.sql included)

🖥 Server Requirement

- Apache Server (XAMPP / WAMP / cPanel)
- PHP 7+
- MySQL 5.6+

📂 Project Structure

```
carrental/
│
├── index.php
├── car-listing.php
├── vehical-details.php
├── search.php
├── my-booking.php
├── profile.php
├── contact-us.php
├── logout.php
│
├── admin/
│   ├── dashboard.php
│   ├── manage-vehicles.php
│   ├── manage-brands.php
│   ├── manage-bookings.php
│   ├── reg-users.php
│   ├── testimonials.php
│   ├── manage-pages.php
│   ├── manage-subscribers.php
│   └── includes/
│
├── includes/
│   ├── config.php
│   ├── header.php
│   └── leftbar.php
│
├── assets/
│   ├── css/
│   ├── js/
│   ├── images/
│   └── fonts/
│
└── carrental.sql
```

🗄 Database Structure & Relations

Main Tables:

tblusers

- id (PK)
- FullName
- EmailId
- Password
- ContactNo

tblvehicles

- id (PK)
- VehiclesTitle
- VehiclesBrand (FK → tblbrands.id)
- PricePerDay
- FuelType
- ModelYear
- SeatingCapacity

tblbrands

- id (PK)
- BrandName

tblbooking

- id (PK)
- userEmail (FK → tblusers.EmailId)
- VehicleId (FK → tblvehicles.id)
- FromDate
- ToDate
- Status

tbltestimonial

- id (PK)
- UserEmail (FK → tblusers.EmailId)
- Testimonial

tblcontactusquery

- id (PK)
- Name
- EmailId
- ContactNumber
- Message

🔗 Database Relationships

- One Brand ➝ Many Vehicles
- One User ➝ Many Bookings
- One Vehicle ➝ Many Bookings
- One User ➝ Many Testimonials

🚀 Installation Guide

- Extract the project folder.
- Place it inside htdocs (XAMPP) or upload to cPanel.
- Create a new database in phpMyAdmin.
- Import carrental.sql.
- Update database credentials in:
  - includes/config.php
- Run the project in browser:
  - http://localhost/carrental
- Admin Panel:
  - http://localhost/carrental/admin

🔐 Default Admin Access (If Included in SQL)

- Admin URL: /admin
- Username: admin
- Password: (check SQL file)

📊 System Advantages

- Fully Dynamic
- Secure Login System
- Responsive Design
- Clean Admin Dashboard
- Easy to Customize
- cPanel Deployment Ready

📌 Future Improvements

- Online Payment Gateway Integration
- Email Notification System
- Role-Based Access Control
- REST API Integration
- Advanced Reporting & Analytics
- Mobile App Version

👨‍💻 Author

- Developed By Md. Shamim Hassan using PHP & MySQL.

