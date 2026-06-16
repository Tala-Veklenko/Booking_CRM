## 🐞 Bug Reports

A set of defects identified during CRM system testing.

📊 Full bug report table:  
[View on Google Sheets](https://docs.google.com/spreadsheets/d/1nP8SRikWiZRDQ8U_e685QJtSKlIGsFeBAujW8juyOT8/edit?usp=sharing)

### Example issues:
- Registration form accepts invalid email format  
- Tour price field allows negative values  
- UI elements misaligned on mobile devices  

### 🐞 Bug Report Example

#### Bug 1: Access control issue

| Field | Value |
|------|------|
| Label | Bug / Access control / Verification status |
| Reporter | Tala Veklenko |
| Summary | Tour operator with “Rejected” status can create tours |
| Reproducibility | 100% |
| OS | macOS |
| Tool/Browser | Postman |
| Precondition | Operator has “Rejected” verification status |

#### Steps to reproduce:
1. Login as tour operator
2. Go to “My Tours”
3. Click “Create new tour”
4. Fill required fields
5. Submit form

#### Actual Result

Tour operator with “Rejected” status can create tours.

#### Expected Result

Access should be restricted until verification is approved.

#### Reason

Access control logic is not properly enforced for rejected users.

#### Severity / Priority
Severity: Major <br>
Priority: High

<br>

---

<br>

#### Bug 2: API returns HTML error response instead of JSON on invalid input

| Field | Value |
|-------|-------|
| Label |Security / API / Error handling|
| Reporter |Tala Veklenko|
| Reproducibility| 100%|
| Screenshot |    |
|OS | macOS |
| Tool |Postman|
| Endpoint | PATCH /api/v1/admin/tours/{id}/feature 


#### Precondition
- User is authenticated  
- User has **ADMIN** role  
- `{id}` refers to an existing tour  
- API endpoint is accessible  

#### Steps to Reproduce
1. Send PATCH request to `/api/v1/admin/tours/{id}/feature`
2. Use request body:
```json id="sec2"
{
  "feature": "'; DROP TABLE tours;--"
}
```
3. Send the request

#### Actual Result
HTTP status code: 403 Forbidden. Response body is returned in HTML format. No structured JSON error response is provided

#### Expected Result
HTTP status code should be 400 Bad Request or 422 Unprocessable Entity
Response body should be returned in JSON format
API should follow consistent error handling contract

#### Severity / Priority
Severity: Major <br>
Priority: High






