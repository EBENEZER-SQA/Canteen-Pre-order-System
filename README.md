# Canteen Pre-Order System

A web app that lets students order food from the campus canteen, pay online, and get an SMS when the order is ready, so there's no more queuing between classes.

## Team
| Name | GitHub | Current role |
|------|--------|--------------|
| EBENEZER SETIAM QUARSHIE AYEDE.| @EBENEZER-SQA | Project manager |
| DERRICK NYAMEKYE | [@KUAMI DERRICK] | Lead developer |
| SOLOBE TIMOTHY  | [@username] | Documentation Lead|
| WILBERFORCE OKYERE | [@username] | Tester |
| ALBERT ALFRED | [@username] | Assistant Tester |

Roles rotate every 3 weeks.

## Features
1. Register and login (student, vendor, admin)
2. Browse the menu, use a cart, place an order
3. Online payment (Paystack test mode)
4. SMS when the order is ready (Africa's Talking sandbox)
5. Vendor dashboard to manage orders and the menu

## Tech stack
PHP, MySQL, HTML/CSS, Bootstrap, JavaScript. Tools: Git, Composer, PHPUnit, Postman.

## Getting started
1. Install XAMPP, Git and Composer.
2. Clone the repo into XAMPP's `htdocs` folder: `git clone [repo-link]`
3. Install dependencies: `composer install`
4. Start Apache and MySQL in XAMPP.
5. In phpMyAdmin, create a database named `canteen_db` and import `database/schema.sql`.
6. Copy `.env.example` to `.env` and fill in your keys. Never commit `.env`.
7. Open `http://localhost/[folder-name]/public`

## Project structure
    canteen-system/
    ├── docs/       SRS, UML, design doc, test plan, risk register, sprint plans
    ├── database/   schema.sql and sample data
    ├── public/     pages the browser opens (index.php, css, js, images)
    ├── src/        PHP code (auth, menu, orders, payments, sms)
    ├── tests/      automated tests
    ├── .env.example
    ├── .gitignore
    ├── composer.json
    └── README.md

## Team workflow
- Never push straight to `main`.
- Branch names: `feature/cart-page`, `fix/login-error`.
- Every pull request is reviewed by another member before merging.
- Commit messages: short and clear, e.g. "Add cart page".

## Testing
Run the automated tests with `vendor/bin/phpunit`

## Documentation
All deliverables are in the `docs/` folder.
