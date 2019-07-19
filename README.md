# POSTMAN CLIENT

### Install and setup
-	Download and install [POSTMAN CLIENT]( https://www.getpostman.com/downloads/)
-	Open the program and import | PATH DIR - QA-FOLDERS / Assessment-DOG-API / Task 1 - API - Public API.json |
-	Steps to take:
    1.	Click on import
    2.	Go to project path and select Task 1 - API - Public API.json
    3.	Click Open

## Test Scenario:

Public API - https://dog.ceo/dog-api/
- Perform an API request to produce a list of all dog breeds.
  (Diagram 1) https://dog.ceo/api/breeds/list/all

- Using code, verify “retriever” breed is within the list
  
  Tests - and click Send Button | it will responds with --- PASS Verify-retriever is within list

(Diagram 2)       
pm.test("Verify-retriever is within list", function () {
    pm.expect(pm.response.text()).to.include("african");
});

- Perform an API request to produce a list of sub-breeds for “retriever”.
  (Diagram 3)  https://dog.ceo/api/breed/retriever/list 

- Perform an API request to produce a random image / link for the sub-breed “golden”
  (Diagram 4)  https://dog.ceo/api/breed/retriever/golden/images/random 
    

## Test Scenario: