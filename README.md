<div align="center">
<p align="center">
  <a href="https://www.php.net/"><img src="https://img.shields.io/badge/PHP-8.0+-blue?logo=php" alt="PHP Badge"></a>
  <a href="https://httpd.apache.org/"><img src="https://img.shields.io/badge/Apache-2.4+-red?logo=apache" alt="Apache Badge"></a>
  <a href="https://www.mysql.com/"><img src="https://img.shields.io/badge/MySQL-8.0+-blue?logo=mysql" alt="MySQL Badge"></a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript"><img src="https://img.shields.io/badge/JavaScript-ES6+-yellow?logo=javascript" alt="JavaScript Badge"></a>
  <a href="https://sass-lang.com/"><img src="https://img.shields.io/badge/SCSS-CSS%20Preprocessor-pink?logo=sass" alt="SCSS Badge"></a>
  <a href="https://jestjs.io/"><img src="https://img.shields.io/badge/Testing-PHPUnit-yellow?logo=testinglibrary" alt="PHPUnit Badge"></a>
</p>
  <a href="https://brandshop.fun/">
    <img src="public/img/favicon/apple-touch-icon.png" alt="logo">
  </a>

<h3 align="center">Brand Shop</h3>
  <p align="center">
This project was created as a study project during an internship at Taitotalo.<br />
    <br />
    <a href="https://brandshop.fun">View website</a>
    .
    <a href="#description">Description</a>
    ·
    <a href="#tech-stack">Tech Stack</a>
     ·
    <a href="#setup">Setup</a>
     ·
    <a href="#testing">Testing</a>
    ·
    <a href="#features">Features</a>
    ·
    <a href="https://github.com/alexelkinx/brand-shop/wiki">Wiki</a>
  </p>
</div>

### Description

The Brand Shop is a web-based application that allows users to browse and purchase fashion items online. The system is designed to provide a user-friendly interface that is easy to navigate and provides an intuitive shopping experience. The platform is fully responsive and optimized for different screen sizes.

### Tech Stack

This project is built using:

- **PHP 8.0+** – server-side scripting
- **Apache 2.4+** – HTTP server
- **MySQL 8.0+** – database
- **JavaScript (ES6+)**
- **SCSS (SASS)**
- **HTML5**

The application follows the Model-View-Controller (MVC) architecture to separate concerns and improve maintainability.

### Setup

To run the Brand Shop locally, make sure you have:

- Apache 2.4 or higher
- PHP 8.0 or higher
- MySQL 8.0 or higher
- Composer (for dependency management)

1. Clone the repository to your local machine:

```bash
  git clone <repository-url>
```

2. Start your local web server (e.g., MAMP or XAMPP).
3. Create a new database in your MySQL server for the project.
4. Import the database from the data-dump.sql file in the project's root/data directory. You can do this by running the following command from the project directory:

```bash
   mysql -u root -p database_name < data-dump.sql
```

Replace `database_name` with the name of the database you created in step 3. You will be prompted to enter your MySQL password.

5. Configure the database connection settings in the config.php file located in the app directory. Replace the DB_HOST, DB_NAME, DB_USER, and DB_PASS values with your MySQL server details.

```php
define('DB_HOST', 'localhost');
define('DB_NAME', 'database_name');
define('DB_USER', 'mysql_username');
define('DB_PASS', 'mysql_password');
```

6. Start your local web server and open the project in your web browser.

   If you placed the project in a subfolder (e.g., `htdocs/brand-shop/`), navigate to:

   http://localhost/brand-shop/

   Adjust the URL depending on your local server setup or custom virtual host configuration.

### Testing

This project uses [PHPUnit](https://phpunit.de/) for automated testing.  
Tests are located in the `/tests` directory and can be run via Composer.

To run the tests:

```bash
composer install     # install dev dependencies, including PHPUnit
composer test        # run all tests with testdox output and color
```

The script is defined in `composer.json` and uses the `--testdox` and `--colors` options for readable and colorized output.

### Features

- **User authentication**: users can sign up, log in (username: `user@email.com` password: `r3YiHfjkniqMfTX`), and log out of the platform.
- **Product catalog**: users can browse the catalog of clothing items and accessories, view product details, and add items to their cart.
- **Shopping cart**: users can view their cart, modify the quantity of items, and remove items from the cart.
- **Checkout process**: users can proceed to checkout, enter their shipping and payment information, and place their order.
- **Order history**: users can view their order history and track the status of their orders.
- **Admin panel**: administrators can log in (username: `admin@admin.com` password: `dVYTRrT7tnkp8BP`) and access the admin panel, where they can manage the product catalog, orders, and users.

### Wiki

More information about the project, including its architecture, ER diagram, sitemap, and webpage layouts: [wiki](https://github.com/alexelkinx/brand-shop/wiki)
