# Database Entity Relationship Diagram (ERD)

## Overview

The SmartRoute AI database is designed using a normalized relational model. The entities are connected through primary and foreign keys to maintain data consistency and integrity.

---

## Entities

### User

Attributes

- user_id (PK)
- first_name
- last_name
- email
- password
- phone
- role
- created_at
- updated_at

---

### Customer

Attributes

- customer_id (PK)
- user_id (FK)
- address
- latitude
- longitude

Relationship

One User → One Customer

---

### Driver

Attributes

- driver_id (PK)
- user_id (FK)
- license_number
- vehicle_id (FK)
- status

Relationship

One User → One Driver

---

### Warehouse

Attributes

- warehouse_id (PK)
- name
- address
- latitude
- longitude

---

### Vehicle

Attributes

- vehicle_id (PK)
- warehouse_id (FK)
- vehicle_number
- type
- fuel_type
- capacity

Relationship

One Warehouse → Many Vehicles

---

### Order

Attributes

- order_id (PK)
- customer_id (FK)
- warehouse_id (FK)
- order_status
- priority
- created_at

---

### Delivery

Attributes

- delivery_id (PK)
- order_id (FK)
- driver_id (FK)
- route_id (FK)
- delivery_status

---

### Route

Attributes

- route_id (PK)
- source
- destination
- distance
- estimated_time
- fuel_cost

---

### Traffic

Attributes

- traffic_id (PK)
- route_id (FK)
- congestion_level
- timestamp

---

### Analytics

Attributes

- analytics_id (PK)
- total_distance
- total_deliveries
- fuel_consumed
- average_delivery_time

---

## Relationship Summary

User
│
├── Customer
│
└── Driver

Warehouse
│
└── Vehicle

Customer
│
└── Order

Order
│
└── Delivery

Driver
│
└── Delivery

Route
│
├── Delivery
│
└── Traffic