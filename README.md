Warehouse Management & Procurement System (WMS + Procurement)

A full-cycle Warehouse Management and Procurement System built with Streamlit, SQLAlchemy, and Python, designed to demonstrate real-world logistics, purchasing, inventory, and financial workflows in a single integrated application.

This project reflects how modern WMS and procurement platforms support end-to-end supply chain operations, from purchase requisitions to goods receipt, inventory valuation, and outbound deliveries.


Live Demo Access (User-Friendly)

This application includes one-click demo access — no credentials required.

Open the app

Click “Demo login” in the sidebar

You are logged in as a Demo Admin user

This allows reviewers to explore all features without setup or configuration.


Key Business Capabilities
Procurement & Purchasing

Purchase requisitions with approval workflow

RFQ (Request for Quotation) creation and supplier bidding

Purchase order generation from winning bids

Full audit trail of procurement actions



Warehouse Management

Multi-warehouse support

Bin locations

Real-time inventory tracking

Automatic inventory updates on goods receipt (IN) and deliveries (OUT)

Inter-warehouse stock transfers




Inbound & Outbound Logistics

Goods receipt notes (GRN)

Quality inspection tracking

Outbound delivery orders

Vehicle and driver assignment



Finance & Compliance:

Invoice capture with line-level detail

Three-way matching (PO ↔ GRN ↔ Invoice)

Payment tracking

Supplier performance scoring




Reporting & Analytics:

Inventory valuation

Spend by supplier

Lead-time analysis (Requisition → GRN)

OTIF (On-Time In-Full) metrics

KPI-ready datasets for operational insights




Role-Based Access Control

The system simulates real enterprise roles:

Requester

Approver

Buyer

Inspector

Finance

Admin

Menu visibility and actions are dynamically controlled based on the logged-in role.
The Demo login uses an Admin role to allow full system exploration.




Technical Architecture
Backend & Data Layer

Python

SQLAlchemy Core

SQLite (default demo mode)

MySQL (optional production setup)

Frontend

Streamlit

Responsive, multi-page layout

Sidebar-based navigation

Design Highlights

Database-agnostic design (SQLite ↔ MySQL)

Automatic schema creation

Transaction-safe operations

JSON audit logging (MySQL compatible)

Clean separation of concerns (auth, inventory, procurement, finance)




Environment  ->  Database                      

Demo / Local ->  SQLite (automatic)            

Production   -> MySQL (via Streamlit Secrets) 



Authentication Model

One-click Demo login (no email/password)

Secure password hashing (SHA-256)

Session-based authentication

Role enforcement across all modules



Deployment

This app is designed for Streamlit Cloud deployment.

No database configuration required for demo

Optional MySQL support via Streamlit Secrets

Safe handling of credentials (no secrets in GitHub)



Why This Project Matters

This project demonstrates:

Practical understanding of WMS & procurement workflows

Strong data modeling and transactional logic

Experience with role-based enterprise systems

Ability to design recruiter-friendly demos

Clean, maintainable Python architecture




Author

Azumi Muhammed
Data Scientist | AI Engineer

Inventory deduction on shipment

