goFood Project README
Project Name: goFood
Overview
goFood is an innovative food ordering system designed to enhance the online food ordering experience. With functionalities like browsing by city, user authentication (login/signup), promotions, reviews, and a dynamic real-time cart, goFood aims to provide a seamless and user-friendly platform for ordering food from various restaurants.

Entity Relationship Diagram (ERD)
The core structure of goFood is based on the following Entity Relationship Diagram (ERD):


Key Features
Browsing by City
Users can browse restaurants based on their city and location. This feature ensures that users can find restaurants that deliver to their specific area.

User Authentication
Users can sign up and log in to the platform. This allows for a personalized experience where users can manage their orders, reviews, and cart.

Promotions
Restaurants can offer promotions that users can apply to their orders. This feature helps in attracting more customers and providing them with better deals.

Reviews
Users can leave reviews for restaurants and their orders. This feedback system helps maintain the quality of service and allows other users to make informed decisions.

Dynamic Real-Time Cart
The cart updates in real-time as users add or remove items. This ensures a smooth and responsive user experience while placing an order.

Database Schema
Location
ID: Unique identifier for each location
STREET: Street address
CITY: City name
STATE: State name
User
ID: Unique identifier for each user
Name: User's name
Email: User's email address
location_id (FK): Foreign key linking to Location
Restaurant
ID: Unique identifier for each restaurant
Name: Restaurant name
description: Description of the restaurant
location_id (FK): Foreign key linking to Location
category_id (FK): Foreign key linking to Category
Category
ID: Unique identifier for each category
name: Name of the category
Order
ID: Unique identifier for each order
user_id (FK): Foreign key linking to User
total_price: Total price of the order
location_id (FK): Foreign key linking to Location
payment_method: Payment method used for the order
Order Items
ID: Unique identifier for each order item
order_id (FK): Foreign key linking to Order
quantity: Quantity of the item ordered
item_id (FK): Foreign key linking to Items
Items
ID: Unique identifier for each item
restaurant_id (FK): Foreign key linking to Restaurant
price: Price of the item
category_id (FK): Foreign key linking to Category
Cart
ID: Unique identifier for each cart
user_id (FK): Foreign key linking to User
Cart Items
ID: Unique identifier for each cart item
cart_id (FK): Foreign key linking to Cart
item_id (FK): Foreign key linking to Items
Review
ID: Unique identifier for each review
user_id (FK): Foreign key linking to User
order_id (FK): Foreign key linking to Order
description: Description of the review





<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

You may also try the [Laravel Bootcamp](https://bootcamp.laravel.com), where you will be guided through building a modern Laravel application from scratch.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains thousands of video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the [Laravel Partners program](https://partners.laravel.com).

### Premium Partners

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[WebReinvent](https://webreinvent.com/)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[DevSquad](https://devsquad.com/hire-laravel-developers)**
- **[Jump24](https://jump24.co.uk)**
- **[Redberry](https://redberry.international/laravel/)**
- **[Active Logic](https://activelogic.com)**
- **[byte5](https://byte5.de)**
- **[OP.GG](https://op.gg)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

