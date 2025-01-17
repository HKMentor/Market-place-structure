**HACKATHON DAY 2
PLANNING THE TECHNICAL FOUNDATION**
HKMentor commented 13 minutes ago
@HKMentor
HKMentor

System Architecture, Workflow, and API Requirements
Building a Seamless Furniture Website

Introduction
_A brief overview of the importance of user-friendly system design and API structure.

“ This presentation explains the system architecture, user workflow, and API design for an e-commerce furniture website. ”

_

System Architecture Overview
1. The system is divided into three components:

Frontend (Next JS, HTML, Tailwind CSS)
Backend (Node.js, API endpoints)
Database (Sanity CMS)

Frontend Requirements
Home Page: Show featured products and promos.
Product Listing: Filter, sort, and fetch products via API.
Product Details: Display title, images, description, and add-to-cart.
Cart Page: Add/remove items, update quantities, and view total.
Checkout Page: Enter details, choose payment, and confirm order.

Main think about our website its is totally responsive design. 


Sanity CMS as Backend
Product Data: Stores product name, title, description, price, image, and category.
Customer Details: Stores customer name, email, phone, and address.
Order Records: Tracks order ID, customer, products, total, and status.


User Workflow
User Registration:
User signs up → Data stored in Sanity → Confirmation sent.
Product Browsing:
User views categories → Sanity API fetches data → Products displayed.
Order Placement:
User adds items to cart → Proceeds to checkout → Order details saved in Sanity.
Shipment Tracking:
Order status fetched via 3rd-party API → Displayed to the user.

Backend Workflow
User Registration:
Receive user data → Store in Sanity → Send confirmation email.
Product Browsing:
Fetch data from Sanity → Display product details to user.
Order Placement:
Receive order details → Store in Sanity → Update order status.
Shipment Tracking:
Call 3rd-party API → Fetch shipment status → Display to user.


### Plan API Requirements

1./products (GET):
{ id: 1, name: "Product A", price: 100, stock: 50, "image": "image_url" }

2./orders (POST):
{ customerInfo: { name: "John Doe", email: "john@example.com" }, productDetails: [{ "id": 1, "quantity": 2 }], paymentStatus: "Paid" }

3./shipment (GET):
{ shipmentId: "12345", orderId: "67890", status: "In Transit", "expectedDelivery"


Third-Party API Structure for e-commerce platform

### Conclusion:

The architecture ensures a seamless user experience, efficient data handling, and scalability for future growth.

This structure supports both technical and business needs for a modern e-commerce system.

THANK YOU
