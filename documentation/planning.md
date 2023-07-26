# Project Planning Documentation for Hip Hop Pizza and Wangs (HHP+W) Proposal Presentation

## Introduction
Welcome to the project planning documentation for Hip Hop Pizza and Wangs (HHP+W). This is an exciting opportunity to build a Point of Sale (POS) application for a well-established restaurant, bringing together the crossroads of music and food. This document outlines the key features, requirements, and guidelines for the HHP+W project.

## Presentation Guidelines
- Each team member will have up to 5 minutes for their proposal presentation, followed by 5 minutes for questions and discussion.
- Submit all presentation information at least 48 hours before the scheduled presentation via the provided link.
- Utilize web presentation software (e.g., Google Slides, Canva, Prezi) to create your presentation and share the links with the instructional team.
- Ensure your proposal clearly articulates the problem HHP+W aims to solve and how your POS application will address their needs.

## Proposal Planning Requirements
- Include a hyperlink to your Entity Relationship Diagram (ERD) accessible to instructors, along with a backup picture of your ERD in case of access issues.
- Hyperlink your wireframes, comprehensively showing the user journey through the POS application.
- Represent each view/page in your wireframes and provide notes or arrows describing user interactions.
- Create a project board outlining your Minimum Viable Product (MVP) using tickets.

## Data Tips from Senior Engineer
During the planning phase, consider the following tips to assist with data management:
- Utilize Firebase Authentication for user authentication in your application.
- Plan your data structure to efficiently manage orders, order items, revenue, and user information.
- Ensure proper validation and error handling for user inputs and form submissions.

## MVP Requirements
Ensure your POS application meets the following Minimum Viable Product (MVP) requirements:
1. Authentication:
   - Users should be able to log in using Google authentication.
   - When logged out, users should see an inviting homepage with a login button.
   - When logged in, users should see a navbar with options to view orders, create an order, and view revenue.

2. Order Management:
   - Users should be able to view a list of all orders with essential details like order name, status, customer contact, and order type.
   - Users should be able to view a list of order items associated with each order, displaying item names and prices.

3. CRUD Operations:
   - Users should be able to create a new order and add order items to it.
   - Users should be able to update order information, including order name, customer contact, and order type.
   - Users should be able to delete an order or an order item from an existing order.

4. Closing Orders and Revenue:
   - Users should be able to close an order by entering payment type and tip amount.
   - Upon closing an order, the order status should change from "Open" to "Closed."
   - Revenue data should be generated upon closing an order, capturing total order amount, date, payment type, and tip amount.
   - Users should be able to view the total revenue made to date.

## General Requirements
Ensure your POS application meets the following general requirements:
- Use clean code with a focus on the Single Responsibility Principle and modular coding.
- Utilize ES6 modules bundled with Webpack for efficient code organization.
- Implement error-free code with clean linters.
- Use Bootstrap 5 for responsive and stylish design elements.
- Plan and organize the project work into tickets and milestones on the Github project board.
- Provide a comprehensive README for the project.

Remember, the MVP aims to deliver a functional POS application that addresses the immediate needs of Hip Hop Pizza and Wangs. Your planning and development should align with the client's requirements and preferences. Good luck with your proposal presentation and project development!
