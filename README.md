Building an Online Bidding System with Spring Boot, React, and MySQL
By Albert Harmon
Published December 24, 2023
4 min read
Technology

TLDRThis blog post provides a comprehensive overview of an online bidding system project developed using Spring Boot, React, and MySQL. It covers the architecture, modules, functionalities, and user interactions within the system, making it a valuable resource for developers and students interested in building similar applications.

In this blog post, we will explore an online bidding system project developed using modern technologies such as Spring Boot, React.js, and MySQL. This project serves as a practical example for developers and students looking to understand how to create a full-fledged online auction system.

Technologies Used
The project utilizes the following technologies:

Backend: Spring Boot (version 3) with Spring Security 6
Frontend: React.js
Database: MySQL
Project Management: Maven
Styling: Bootstrap
The development environment includes:

Backend Development: Spring Tool Suite (STS)
Frontend Development: Visual Studio Code (VS Code)
Database Management: MySQL Workbench
Project Overview
The online bidding system consists of two main modules:

Administrator Module
Customer Module
Functional Modules
The project includes several functional modules:

User Authentication Module: Handles user registration and login.
Customer Module: Allows customers to bid on products and manage their accounts.
Delivery Module: Manages delivery personnel and their assignments.
Product Module: Handles product listings and details.
Bidding Module: Manages the bidding process for products.
Order Module: Tracks orders and their statuses.
Wallet Module: Manages customer wallets for bidding transactions.
User Roles
In this system, the roles of seller and buyer are combined into the customer module. After logging in, a customer can both sell products and bid on others. The process begins with customer registration, followed by product listing and bidding.

How the Bidding Process Works
Customer Registration: Customers register and log in to the system.
Product Listing: To sell a product, the customer must first register a delivery person. After that, they can add product details, including the asking price and expiry date. The product will automatically disappear from the system once the bidding period ends, going to the highest bidder.
Bidding: Multiple buyers can bid on a product, with bids needing to exceed the asking price. The highest bid at the expiry time wins the product.
Order Management: Once a product is allocated to a buyer, both the buyer and seller can view the order details. The seller can assign a delivery person for the product delivery.
Delivery Tracking: The delivery person can log in to see their assigned deliveries and update the delivery status.
Wallet Management: Buyers must have sufficient funds in their wallets to place bids. The bid amount is deducted from the buyer's wallet and credited to the seller's wallet upon successful bidding.
Administrator Functions
The administrator has access to a dashboard that provides complete details about sellers, delivery personnel, buyers, and products. Key functionalities include:

Registering new administrators
Adding, updating, and deleting product categories
Viewing all orders and their statuses
Managing delivery personnel and customer accounts
Customer Functions
Customers can perform various actions, including:

Adding funds to their wallet
Bidding on products
Viewing their bids and orders
Adding products for sale
Managing delivery personnel for their products
Project Structure
The project is structured into several packages, including:

Config: Configuration settings for the application.
Controller: Handles incoming requests and responses.
DTO: Data Transfer Objects for data handling.
Entity: Represents the database entities.
Exception Handler: Manages exceptions throughout the application.
JWT Filter: Handles JSON Web Token authentication.
Running the Project
To run the project, both the backend and frontend applications need to be started. The backend can be run using Spring Tool Suite, while the frontend can be started using npm in the terminal. Once both applications are running, users can interact with the online bidding system through the web interface.

Conclusion
This online bidding system project showcases the integration of various technologies to create a functional and user-friendly auction platform. It serves as an excellent learning resource for students and developers looking to enhance their skills in web development and project management. By understanding the architecture and functionalities of this project, you can apply similar concepts to your own projects.

If you found this overview helpful, consider exploring the project further or using it as a foundation for your own development endeavors.
