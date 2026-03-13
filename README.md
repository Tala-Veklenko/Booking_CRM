# CRM System Testing Project

This repository contains testing documentation for a CRM system used by travel agencies.

The system allows:
- users to search and book tours
- tour operators to manage tour offers
- administrators to manage users and system data

During this project I performed manual testing of both frontend and backend functionality.

## Roles Tested

Testing was performed from three user perspectives:

User
- search tours
- view tour details
- create bookings

Tour Operator
- create and edit tours
- manage bookings
- update pricing and availability

Admin
- manage users
- monitor system data
- control permissions

## Scope of Testing

The following types of testing were performed:

Frontend Testing
- Cross-browser testing (Chrome, Firefox, Safari)
- UI validation using Figma designs
- DevTools for network, console, and performance checks
- Frontend-backend data consistency verification

Beckend testing
- REST API (manual testing via Postman)
- Booking & payment business logic
- Input validation and API contract
- Pagination and data consistency
- Authorization and security (OWASP Top 10 basics)

## Test Documentation

Test documentation includes:

- Test plan
- Test cases
- Checklists
- Bug reports

All documentation can be found in the corresponding folders.

## Tools Used

- ClickUp (bug tracking simulation)
- Postman (API testing)
- Swagger (API collection)
- Chrome DevTools
- Google Sheets (documentation)
- CHatGPT (support)

## Example Bugs Found

Examples of issues identified during testing:

1. Registration form allows invalid email format
2. Tour price field accepts negative values
3. "Add to booking" button not visible on mobile screens
4. API returns incorrect status code for invalid request

Detailed bug reports are available in the Bug-Reports folder.

## Test Cases

More than 20 test cases were created covering:

- booking flow
- role permissions
- CRUD operations for tours
- user management

See Test-Cases.md for details.

## Author

Manual QA portfolio project created to demonstrate testing skills and documentation.

