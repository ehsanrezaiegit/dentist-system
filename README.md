# 🦷 Dentist Appointment System

A comprehensive and robust Dentist Appointment Management System built with **Laravel**. This project provides a complete solution for managing dental clinic operations, including patient reservations, doctor schedules, and an administrative dashboard.

Features

*   **User Roles & Authentication:** Secure login and registration for Patients, Doctors, and Administrators.
*   **Admin Dashboard:** Centralized panel to manage users, doctors, and monitor all clinic appointments.
*   **Appointment Booking:** Seamless reservation system for patients to book available time slots.
*   **Conflict Prevention:** Smart validation to prevent overlapping appointments for the same doctor.
*   **Responsive UI:** Modern, clean, and responsive user interface styled with **Tailwind CSS** and **Alpine.js**.
*   **Secure:** Built-in protection against CSRF and XSS attacks, featuring custom middleware for role-based access control.

## 🛠️ Tech Stack

*   **Backend:** [Laravel](https://laravel.com/) (PHP)
*   **Frontend:** [Tailwind CSS](https://tailwindcss.com/), [Alpine.js](https://alpinejs.dev/), Blade Templates
*   **Database:** MySQL / PostgreSQL
*   **Architecture:** MVC (Model-View-Controller)

## ⚙️ Installation & Setup

Follow these steps to set up the project on your local Ubuntu or WSL environment:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/dentist-system.git
    cd dentist-system
    ```

2.  **Install PHP dependencies:**
    ```bash
    composer install
    ```

3.  **Install Node.js dependencies (for Tailwind/Alpine):**
    ```bash
    npm install
    npm run build
    ```

4.  **Environment Setup:**
    Copy the example env file and configure your database credentials.
    ```bash
    cp .env.example .env
    ```

5.  **Generate Application Key:**
    ```bash
    php artisan key:generate
    ```

6.  **Run Migrations:**
    Configure your `.env` database settings, then run:
    ```bash
    php artisan migrate
    ```

7.  **Start the Development Server:**
    ```bash
    php artisan serve
    ```
    Access the application at `http://localhost:8000`.

## 📂 Project Structure Highlights
*   `app/Http/Controllers/Admin/`: Dedicated controllers for administrative logic.
*   `app/Http/Middleware/AdminMiddleware.php`: Custom security layer protecting admin routes.
*   `database/migrations/`: Database schema definitions ensuring solid relational structures (Doctors, Patients, Appointments).

## 📝 License

This project is open-source and available under the [MIT license](https://opensource.org/licenses/MIT).
