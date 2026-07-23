# Class Diagram

Main Classes

User

Customer

Driver

Warehouse

Vehicle

Order

Delivery

Route

Traffic

Analytics

Graph

Node

Edge

Algorithms

Dijkstra

AStar

BFS

DFS

FloydWarshall

Prim

Kruskal

PriorityQueue

Relationships

User
├── Customer
└── Driver

Warehouse
└── Vehicle

Customer
└── Order

Order
└── Delivery

Driver
└── Delivery

Delivery
└── Route

Route
├── Graph
└── Traffic