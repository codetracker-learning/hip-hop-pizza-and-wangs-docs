# Ticket Descriptions - Hip Hop Pizza and Wangs (HHP+W) POS Application

The following ticket descriptions have been created based on the discussions held with the client (Hip Hop Pizza and Wangs) regarding the development of a Point of Sale (POS) application. These tickets outline specific functionalities and requirements for the project and serve as a guide for the development team working on the implementation.

**Ticket Descriptions - Hip Hop Pizza and Wangs (HHP+W) POS Application**

These tickets have been written to capture the key features and functionalities discussed during the client meetings. Each ticket provides a clear description of the desired behavior, including the given conditions, expected actions, and resulting outcomes. The potential implementation ideas offer suggestions for the technical approach that can be considered.

These tickets will serve as a reference for the development team, ensuring accurate implementation of the discussed features. The project manager will work closely with the development team to prioritize and track the progress of each ticket.

Please review these ticket descriptions to gain a comprehensive understanding of the project's scope and objectives as conveyed by the client.

## Title: Authentication and User Management

- **Given** that the user is logged out
- **When** the app first loads
- **Then** they should see a home screen with either an h1 or the Logo displaying "Hip Hop Pizza and Wings" (create `homeLoggedOut` component)
- **And** a button to log in

- **Given** that the user is logged in
- **When** the app first loads
- **Then** they should see a navbar with a brand and a logout button
- **And** a link to view all orders in the navbar
- **And** a link to Create an Order in the navbar
- **And** an H1 on the page that says, "Welcome, [username]!" (create `homeLoggedIn` component)
- **And** buttons to view orders, create an order, and view revenue

## Title: READ - Display List of Orders

- **Given** an authenticated user
- **When** the user clicks on "View Orders"
- **Then** they should see a list of all orders
- **And** each order should display order name, status (open or closed), customer phone number, customer email address, and order type

## Title: READ - Display Order Details and Associated Order Items

- **Given** an authenticated user
- **When** the user clicks on a specific order
- **Then** they should see the order details
- **And** a list of all order items associated with the order
- **And** each order item should display order item name and price

## Title: DELETE - Delete Order Item and Order

- **Given** an authenticated user
- **When** the user clicks on the "Delete" button for an order item
- **Then** the order item should be deleted from the order

- **Given** an authenticated user
- **When** the user clicks on the "Delete" button for an order
- **Then** the order should be deleted
- **And** all order items associated with that order should be deleted as well

## Title: CREATE - Create an Order

- **Given** an authenticated user
- **When** the app first loads
- **Then** they should see a home screen with a button that reads "Create Order"
- **And** when the user clicks the "Create Order" button
- **Then** they should be able to create a new order
- **And** they should be able to add order items to the order

## Title: UPDATE - Update Order Information

- **Given** an authenticated user
- **When** the user is looking at an order
- **Then** they should be able to update order name, customer phone number, customer email address, and order type

## Title: UPDATE - Update Order Item Information

- **Given** an authenticated user
- **When** the user is looking at an order item
- **Then** they should be able to update item name and item price

## Title: Close Order and Generate Revenue

- **Given** an authenticated user
- **When** the user is looking at an order
- **And** they click a button to go to the Close Order Form
- **Then** they should be able to input payment type (cash, check, debit, credit, or mobile-payment) and tip amount
- **And** when the user submits the Close Order Form
- **Then** the order's status should change from "Open" to "Closed"
- **And** a new revenue node should be created with total order amount (including tip), date, payment type, and tip amount

## Title: View Revenue

- **Given** an authenticated user
- **When** the app first loads
- **Then** they should see a home screen with a button that reads "View Revenue"
- **And** when the user clicks the "View Revenue" button
- **Then** they should be able to see the sum of all revenue made to date

### Potential Implementation Ideas:

- The app could use Firebase for authentication and data storage.
- Each order could be represented as a separate document in the Firebase Firestore database.
- Each order item could be a subcollection under the order document, storing the item name and price.
