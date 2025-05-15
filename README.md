# My First PHP Framework (ESTIAM Bourges Project)

Welcome to my first PHP framework! This project was developed as part of my first-year studies at ESTIAM Bourges. It's a MVC (Model-View-Controller) framework built from scratch using PHP 8.4 and MariaDB, designed to handle basic web application functionalities, including CRUD operations for managing students.
## 🌟 Features

*   **MVC Architecture:** Organizes code into Models (for data logic via `core/model.php`), Views (for presentation in `src/views/`), and Controllers (for request handling in `src/controllers/`).
*   **Database Interaction (PDO):** Uses PDO for database communication.
    *   `core/DB.php` handles the database connection.
    *   `core/model.php` provides base methods like `find()`, `insert()`, `update()`, and `delete()`.
*   **Query Building (`core/Requester.php`):** A custom `Requester` class assists in constructing SQL query strings.
*   **CRUD Operations:** Demonstrates Create, Read, Update, and Delete functionalities for a `students` entity.
    *   **Create:** `studentController::add()` for form, `studentController::postadd()` for submission.
    *   **Read:** `studentController::index()` for listing, `studentController::index()` for fetching.
    *   **Update:** `studentController::edit()` for form, `studentController::postedit()` for submission.
    *   **Delete:** `studentController::delete()` handles AJAX requests for deletion.
*   **Simple View Rendering:** The base `Controller` class provides `render()` and `set()` methods to pass data to PHP-based view files.
*   **AJAX for Deletion:** The student listing page (`src/views/student/index.php`) uses JavaScript `fetch` for deletion.
*   **Basic Styling:** Includes a `public/css/style.css` for the user interface.

## 🛠️ Tech Stack & Requirements

*   **PHP:** 8.4
*   **Database:** MariaDB
*   **Web Server:** Apache (recommended due to WAMP usage).

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites

*   A local web server environment (e.g., WAMP, XAMPP, MAMP).
*   PHP 8.4 installed and configured.
*   A MariaDB database server.

### Installation

1.  **Clone the repository:**
    
