# CRUD-operations-table
A simple CRUD API built with FastAPI to manage person records.
Supports Create, Read, Update, Delete operations using an in-memory dictionary (acts like a database).

🚀 Features-
➕ Add a new person
📋 Get all persons
🔎 Get person by ID
✏️ Update existing person details
❌ Delete a person

API endpoints- 
| Method     | Endpoint       | Description           | Request Body Example                                                        |
| ---------- | -------------- | --------------------- | --------------------------------------------------------------------------- |
| **POST**   | `/person/`     | Add a new person      | `{ "id": 1, "name": "Sameer", "age": 23, "email": "sameer@example.com" }`   |
| **GET**    | `/persons/`    | Get all persons       | –                                                                           |
| **GET**    | `/person/{id}` | Get person by ID      | –                                                                           |
| **PUT**    | `/person/{id}` | Update person details | `{ "id": 1, "name": "Updated", "age": 24, "email": "updated@example.com" }` |
| **DELETE** | `/person/{id}` | Delete a person by ID | –                                                                           |

Save code as main.py
Run the server
uvicorn main:app --reload

Open in browser:
Local host - ( http://127.0.0.1:8000/ )
Swagger UI 👉( http://127.0.0.1:8000/docs )
ReDoc 👉( http://127.0.0.1:8000/redoc )

How to Use It (Guide)
Once the browser page opens (/docs), you will see buttons for different actions:
Add a Person (POST /person/)
Click on POST /person/
Click “Try it out”
Fill in details (id, name, age, email)
Click Execute
🎯 Result: Person is saved in memory
See All Persons (GET /persons/)
Click on GET /persons/
Click Execute
🎯 Result: Shows list of all saved persons
Find Person by ID (GET /person/{id})
Click GET /person/{person_id}
Enter the ID (example: 1)
Click Execute
🎯 Result: Shows details of that one person
Update Person (PUT /person/{id})
Click PUT /person/{person_id}
Enter ID of the person you want to update
Change details in the form (example: new age)
Click Execute
🎯 Result: Person’s record is updated
Delete Person (DELETE /person/{id})
Click DELETE /person/{person_id}
Enter ID (example: 1)
Click Execute
🎯 Result: Person record is deleted
