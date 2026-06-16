# 🧪 CRM System Testing Project

This repository contains QA documentation for a CRM system used by travel agencies.

The system supports:
- searching and booking tours
- tour management by operators
- user and system management by administrators

This project demonstrates end-to-end manual testing of frontend and backend functionality across multiple user roles.

---
## 📁 Repository Structure

- test-cases/
- bug-reports/
- checklists/
- api/
- test-design/

---
## 👤 Roles Tested

### 🧑 User
- Search and filter tours
- View tour details
- Create bookings

### 🧑‍💼 Tour Operator
- Create and update tours
- Manage bookings
- Update pricing and availability

### 🛠 Admin
- Manage users
- Control system permissions
- Monitor system data

---

## 🧪 Testing Scope

### 🖥 Frontend Testing
- Cross-browser testing (Chrome, Firefox, Safari)
- UI validation against Figma designs
- DevTools usage (network, console, performance)
- Data consistency between UI and backend

### 🔌 Backend Testing
- REST API testing (Postman, Swagger)
- Booking and payment business logic validation
- Input validation and boundary testing
- Pagination and data integrity checks
- Basic security testing (authentication & authorization)

---

## 📂 Test Documentation

The project includes the following artifacts:

- Test Plan
- Test Cases
- Checklists
- Bug Reports
- API Collections (Postman)

All files are available in the corresponding repository folders.

---

## 🛠 Tools Used

- Postman — API testing
- Swagger — API documentation
- Chrome DevTools — debugging & network analysis
- ClickUp — bug tracking
- Google Sheets — test documentation
- ChatGPT — support for test idea generation

---

## 🐞 Example Defects Found

- Registration form accepts invalid email formats
- Tour price field allows negative values
- "Add to booking" button is missing on mobile devices
- API returns incorrect HTTP status codes for invalid requests

Full bug reports are available in the `bug-reports/` folder.

---

## 📊 Test Coverage

- Booking flow
- Role-based access control
- CRUD operations for tours
- User management
- Payment workflow validation

---

## 👩‍💻 Author

This project was created as part of a QA portfolio to demonstrate:
- Manual testing skills
- API testing experience
- Test documentation practices
- Understanding of STLC
