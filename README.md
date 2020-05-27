# Stolen Cars
1. There are two folder Backend/Frontend.
2. Backend contains the APIs logics.
3. Fronent contain the Frontend react app.
4. For DB I am using mlab mongo instance.

### To RUN THIS PROJECT
1. RUN npm install in root folder.
2. RUN npm install in both Backend and Frontend folder.
3. RUN npm start in root folder to start the app.
4. Frontend will runs on localhost:3000
5. Backend will runs on localhost:3001

## APIs
1. <b> Get complaints: This gives the list of all registered complaints.</b><br>
Endpoint: localhost:3001/complaints/<br>
Method: GET

2. <b>Create New complaint: This api is used to add new complaint. </b> <br>
Endpoint: localhost:3001/complaints/new <br>
Method: POST <br>
Body: {
    "ownerName": "",
	"ownerNumber": "",
    "carColor": "",
    "carNumber": "",
    "carModel": "",
    "manufacturingYear": "",
    "carChassis": ""
} 

3. <b> Get officers: This gives the list of all officers</b><br>
Endpoint: localhost:3001/complaints/<br>
Method: GET <br>
Note: officerId, Name can be used as a query to fetch officer.


4. <b> Create new officer: This api is use to create new officer </b> <br>
Endpoint: localhost:3001/officers/new
Method: POST <br>
Body: {
    "name": "",
    "dateOfBirth": "",
    "address": "",
    "phoneNumber": ""
}

5. <b> Resolve complaint: This api is used to resolve the complaint.</b><br>
Endpoint: localhost:3001/officers/:officerId <br>
Method: POST
Body: {} 

## Notes
1. Officer is automatically assigned to the application as per the requirement. This is random assignment you can find the assignment logic in helper.js file.


