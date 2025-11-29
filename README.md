# Online Mobile Purchasing System

## Overview
This is a WordPress-based online mobile shop system developed as a project for the Bachelor of Engineering in Computer Engineering at Khwopa Engineering College, Purbanchal University. It allows users to browse, select, and purchase mobile products online, with features like user registration, admin management, shopping cart, checkout, and secure transactions.

Key features:
- User browsing and ordering of mobile products.
- Admin panel for editing menu items, product details, and authorization.
- Secure login/registration.
- Shopping cart and easy billing.
- Responsive design for desktops, tablets, and smartphones.
- User reviews and feedback system.

Built with WordPress and WooCommerce (based on database tables like `wp_woocommerce_*`).

## Setup Instructions

### Prerequisites
- PHP 8.2+ (as per DB dump)
- MySQL/MariaDB 10.4+
- Apache/Nginx server (e.g., XAMPP, MAMP, or local dev environment)
- WordPress (core files included, but recommend fresh install for updates)

### Installation
1. Clone the repo:
  git clone https://github.com/praful10214/Online-Mobile-Shop-wp.git
  cd online-mobile-shop-wp

2. Set up database:
- Create a MySQL database named `mysite`.
- Import `mysite.sql` (if not ignored) via phpMyAdmin or command line:
  mysql -u root -p mysite < mysite.sql

3. Configure WordPress:
- Copy `wp-config-sample.php` to `wp-config.php`.
- Edit `wp-config.php` with your DB details:
  define('DB_NAME', 'mysite');
define('DB_USER', 'root');  // Or your DB user
define('DB_PASSWORD', '');  // Set a secure password
define('DB_HOST', 'localhost');
 - Update salts/keys from https://api.wordpress.org/secret-key/1.1/salt/.

4. Set up file permissions:
- `wp-content/` should be writable (755 or 775).

5. Access the site:
- Place files in your server root (e.g., htdocs for XAMPP).
- Visit `http://localhost/`...
- Admin login: Use credentials from project 

6. Install dependencies:
- If using Composer: `composer install` (add composer.json if needed for plugins).
- Activate WooCommerce and any custom themes/plugins via WP admin.

### Usage
- **Frontend**: Browse mobiles, add to cart, checkout.
- **Admin**: Login at `/wp-admin/` to manage products, orders, users.
- **Pages**: Includes Home, Shop, Checkout, Cart, About Us, Contact Us.
- **Technologies**: WordPress, PHP, MySQL, WooCommerce (inferred from DB structure), HTML/CSS/JS.

### Development
- Custom theme/plugin in `wp-content/'.
- Debug: Set `WP_DEBUG` to true in `wp-config.php`.
- Updates: Keep WP core, themes, and plugins updated.

🧑‍💻 Author
- Praful Man Thaku
- Frontend Developer
- GitHub: praful10214
- Email: praful.thaku@gmail.com

### License
This project is licensed under the GNU General Public License v2 (or later) as per WordPress. See `license.txt` for details.
