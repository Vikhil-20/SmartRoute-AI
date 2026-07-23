# Database Design

Main Tables

- users
- customers
- drivers
- warehouses
- vehicles
- orders
- routes
- deliveries
- traffic
- analytics

Relationships

User
  |
  +---- Customer

User
  |
  +---- Driver

Warehouse
   |
   +---- Vehicles

Order
   |
   +---- Delivery

Delivery
   |
   +---- Route

Route
   |
   +---- Graph