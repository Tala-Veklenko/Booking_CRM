# Backend QA Portfolio – Booking CRM

This repository contains examples of my QA work on a Booking CRM pet project.

## Frontend Testing
- Cross-browser testing (Chrome, Firefox, Safari)
- UI validation using Figma designs
- DevTools for network, console, and performance checks
- Frontend-backend data consistency verification

## Beckend testing
- REST API (manual testing via Postman)
- Booking & payment business logic
- Input validation and API contract
- Pagination and data consistency
- Authorization and security (OWASP Top 10 basics)

## Artifacts
- Bug reports (Markdown + full PDF list)
- Postman collections with API tests
- Test strategy and notes

## Key Findings
- IDOR vulnerability in booking creation
- Authorization bypass for admin endpoints
- Missing validation causing 500 errors
- Inconsistent pagination due to missing ORDER BY
- Price calculation mismatch (frontend vs backend)



## POSTMAN collection
GitHub folder structure for JSON collections of API tests

API-test_collection/ <br>
└── Tours/ <br>
    ├── POST_createTour.json      # Create new tour <br>
    ├── GET_getTours.json         # Get list of tours <br>
    ├── GET_getTourById.json      # Get tour by ID <br>
    ├── PATCH_updateTour.json     # Update tour <br>
    ├── DELETE_deleteTour.json    # Delete tour <br>
    ├── PATCH_updatePhoto.json    # Update photo for tour <br>
    └── DELETE_deletePhoto.json   # Delete photo for tour <br>
        


