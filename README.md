# 🚗 WhatNext Vision Motors – Salesforce Vehicle Management System

## 📌 Project Overview

**WhatNext Vision Motors** is a Salesforce-based vehicle management and customer relationship solution developed to streamline vehicle ordering, dealership operations, customer management, and vehicle-related services.

The system centralizes vehicle, dealer, customer, vehicle order, test drive, and service request information using Salesforce custom objects, fields, relationships, Lightning App Manager, Flow automation, Apex, Reports, and Dashboards.

A key automation is a **Record-Triggered Flow** that automatically assigns a vehicle order to the appropriate dealer based on the customer's location.

---

## 🎯 Project Objectives

- Centralize vehicle, dealer, customer, and order information.
- Manage vehicle inventory and stock information.
- Automate vehicle order processing.
- Automatically assign orders to the appropriate dealer.
- Validate vehicle stock availability.
- Reduce manual intervention in dealership operations.
- Improve data organization and order accuracy.
- Automate business processes using Salesforce Flow and Apex.
- Provide Reports and Dashboards for operational monitoring.
- Provide a dedicated Lightning application for vehicle management.

---

## 🧩 Salesforce Data Model

| Object | Purpose |
|---|---|
| **Vehicle** | Stores vehicle details and stock information. |
| **Vehicle Dealer** | Stores dealer details, location, contact information, and dealer code. |
| **Vehicle Customer** | Stores customer details and preferences. |
| **Vehicle Order** | Tracks vehicle purchases and order status. |
| **Vehicle Test Drive** | Manages customer test-drive bookings. |
| **Vehicle Service Request** | Manages customer service requests. |

### 🔗 Key Relationships

- Vehicle → Dealer and Vehicle Orders
- Vehicle Dealer → Vehicle Orders
- Vehicle Customer → Vehicle Orders and Test Drives
- Vehicle Order → Customer, Vehicle, and Dealer
- Test Drive → Customer and Vehicle
- Service Request → Customer and Vehicle

---

## ⚙️ Automation

### 🔄 Record-Triggered Flow – Auto Assign Dealer

The project uses a **Record-Triggered Flow** to automate dealer assignment.

### Process

1. A Vehicle Order is created with status **Pending**.
2. The Flow retrieves the related **Vehicle Customer**.
3. The Flow retrieves the appropriate **Vehicle Dealer** based on the customer's location.
4. The Flow updates the Vehicle Order with the assigned dealer.
5. The order continues through the automated processing workflow.

### Other Automation

- Stock availability validation
- Vehicle order processing
- Dealer assignment
- Order and status updates
- Apex Triggers
- Batch processing
- Inventory updates

---

## 🧑‍💻 Salesforce Features Used

- Salesforce CRM
- Salesforce Developer Edition
- Custom Objects
- Custom Fields
- Lookup Relationships
- Picklist Fields
- Lightning App Manager
- Salesforce Flow
- Record-Triggered Flow
- Auto-Launched Flow
- Apex Classes
- Apex Triggers
- Batch Apex
- Reports
- Dashboards
- Profiles
- Permission Sets
- Role Hierarchy
- Sharing Rules
- Field-Level Security

---

## 📱 Lightning Application

A dedicated **WhatNext Vision Motors** Lightning application provides centralized access to the vehicle management modules.

### Navigation Items

- 🚗 Vehicles
- 🏢 Dealers
- 👤 Customers
- 📦 Orders
- 🚘 Test Drives
- 🛠️ Service Requests
- 📊 Reports
- 📈 Dashboards

---

## 🔐 Security

The project includes Salesforce security and access-control concepts such as:

- Profiles
- Permission Sets
- Role Hierarchy
- Sharing Rules
- Field-Level Security
- Object-Level Security
- Record-Level Access

These features help ensure that users have appropriate access to the required Salesforce data and functionality.

---

## 📊 Reports & Dashboards

Reports and Dashboards are used to monitor:

- Vehicle inventory
- Vehicle stock levels
- Vehicle orders
- Order status
- Dealer information
- Customer information
- Dealer performance
- Operational metrics

---

## 🏗️ Solution Architecture

```text
                    WHATNEXT VISION MOTORS
                         Salesforce CRM
                              |
          +-------------------+-------------------+
          |                   |                   |
          v                   v                   v
   Custom Objects       Lightning App         Security
          |                   |                   |
   Vehicle / Dealer     Vehicles / Dealers   Profiles
   Customer / Order     Orders / Reports     Permission Sets
   Test Drive / Service Dashboards           Sharing Rules
          |
          v
     Vehicle Order
          |
          v
   Record-Triggered Flow
          |
    +-----+----------+
    |                |
    v                v
 Customer Lookup   Dealer Lookup
    |                |
    +-------+--------+
            |
            v
      Dealer Assignment
            |
            v
        Apex / Batch
            |
            v
     Reports & Dashboards
```

---

## 📋 Project Planning

The project follows an **Agile methodology** using:

- Epics
- User Stories
- Story Points
- Sprint-based execution
- Velocity calculation
- Project milestones

### Major Development Areas

1. Salesforce Environment Setup
2. Data Modeling
3. Custom Objects and Relationships
4. Fields and Tabs
5. Lightning App Development
6. Flow Automation
7. Apex Development
8. Reports and Dashboards
9. Security Configuration
10. Testing and Deployment

---

## 🧪 Testing

Testing covers:

- Vehicle creation
- Customer creation
- Dealer creation
- Vehicle Order creation
- Pending order processing
- Dealer assignment
- Stock availability validation
- Apex execution
- Batch processing
- Reports
- Dashboards
- User access and security

---

## 🌟 Key Benefits

- Centralized vehicle and dealership data
- Automated vehicle order processing
- Automated dealer assignment
- Reduced manual processing
- Improved data organization
- Better order management
- Improved inventory visibility
- Better operational monitoring
- Scalable Salesforce-based architecture

---

## 🔮 Future Scope

The project can be enhanced with:

- Advanced vehicle recommendation features
- Improved dealer-distance calculation
- Customer notifications
- Enhanced inventory forecasting
- Additional dashboards and analytics
- Mobile-oriented user experience
- External vehicle/inventory system integration
- AI-assisted customer support
- AI-based vehicle recommendations

---

## 🛠️ Technology Stack

| Category | Technology |
|---|---|
| CRM Platform | Salesforce |
| Development Environment | Salesforce Developer Edition |
| User Interface | Salesforce Lightning |
| Automation | Salesforce Flow |
| Backend | Apex |
| Database | Salesforce Custom Objects |
| Security | Profiles, Permission Sets, Sharing Rules, Field-Level Security |
| Analytics | Reports & Dashboards |

---

## 📂 Project Structure

```text
WhatNext-Vision-Motors/
│
├── README.md
│
├── Documentation/
│   └── WhatNext Vision Motors Project Report.pdf
│
├── Screenshots/
│   ├── vehicle-object.png
│   ├── vehicle-dealer.png
│   ├── vehicle-customer.png
│   ├── vehicle-order.png
│   ├── lightning-app.png
│   ├── auto-assign-dealer-flow.png
│   ├── apex-classes.png
│   ├── reports.png
│   └── dashboards.png
│
└── Salesforce/
    └── Project Source Files
```

---

## 📸 Screenshots

Screenshots of the Salesforce implementation can be added to the `Screenshots/` folder.

### Vehicle Object

```markdown
![Vehicle Object](Screenshots/vehicle-object.png)
```

### Vehicle Dealer

```markdown
![Vehicle Dealer](Screenshots/vehicle-dealer.png)
```

### Vehicle Customer

```markdown
![Vehicle Customer](Screenshots/vehicle-customer.png)
```

### Vehicle Order

```markdown
![Vehicle Order](Screenshots/vehicle-order.png)
```

### Lightning Application

```markdown
![WhatNext Vision Motors Lightning App](Screenshots/lightning-app.png)
```

### Auto Assign Dealer Flow

```markdown
![Auto Assign Dealer Flow](Screenshots/auto-assign-dealer-flow.png)
```

---

## 🎥 Project Demo

### 🔗 Demo Link

**[▶️ View WhatNext Vision Motors Project Demo](PASTE-YOUR-DEMO-LINK-HERE)**

> Replace `PASTE-YOUR-DEMO-LINK-HERE` with your actual demo link.

Example:

```markdown
[▶️ View Project Demo](https://your-demo-link-here.com)
```

---

## 📄 Project Documentation

The complete project documentation covers:

- Project Overview
- Problem Statement
- Requirement Analysis
- Customer Journey
- Solution Architecture
- Project Planning
- Salesforce Implementation
- Custom Objects
- Fields and Relationships
- Lightning App
- Flow Automation
- Apex Development
- Security
- Reports
- Dashboards
- Testing
- Conclusion
- Future Scope

---

## 👥 Team

### Team ID

**SWTID-2026-2934**

### Team Members

| Role | Name | Email |
|---|---|---|
| 👑 Team Lead | **Sriragh SS** | sriragh1432005@gmail.com |
| 👨‍💻 Team Member | **Mohammed Zaid Affan H** | zaidaffan456@gmail.com |
| 👨‍💻 Team Member | **Prajit S** | prajitprajit59@gmail.com |
| 👨‍💻 Team Member | **LalithRam DJ** | lalithramdj@gmail.com |
| 👨‍💻 Team Member | **Ramprabu M** | ramprabu1802@gmail.com |

---

## 🏫 Institution

**Alpha College Of Engineering**

---

## 📌 Project Status

The **WhatNext Vision Motors – Salesforce Implementation** covers the core vehicle-management data model, custom objects and relationships, Lightning application configuration, Flow automation, Apex development, security configuration, Reports, and Dashboards.

The repository can be extended with additional Salesforce source files, screenshots, documentation, and project demonstration materials.

---

## 📄 License

This project was developed as an academic/project implementation using Salesforce technologies.

---

## ⭐ Acknowledgement

This project was developed as part of the Salesforce-based vehicle management implementation project **WhatNext Vision Motors**.

---

# 🚗 WhatNext Vision Motors

### *Shaping the Future of Mobility with Innovation and Excellence*
