# Notes API – Java & Spring Boot

A robust RESTful API for secure note management, built with Java 17, Spring Boot, and an in-memory H2 database.  
This project demonstrates key backend development skills: CRUD operations, validation, persistence, and API testing.

## 🚀 Features

- Create, Read, Update, and Delete notes via RESTful endpoints
- Automatic creation timestamp for every note
- Data validation: Title and content cannot be blank
- Proper error handling for invalid data or missing notes

## ⚙️ How to Run

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/notesapi.git
   cd notesapi
   ./mvnw spring-boot:run // start the application 
   
or directly run
```sh
    NotesapiApplication.java


---

## 5️⃣ **Document Your API Endpoints**

```markdown
## 🛠️ API Endpoints

| Method | Endpoint         | Description          |
|--------|------------------|---------------------|
| POST   | /notes           | Create a note       |
| GET    | /notes           | List all notes      |
| GET    | /notes/{id}      | View a single note  |
| PUT    | /notes/{id}      | Update a note       |
| DELETE | /notes/{id}      | Delete a note       |

### Example: Create a Note

**Request:**
```json
POST /notes
{
  "title": "Grocery List",
  "content": "Eggs, Milk, Bread"
}
Response:
{
  "id": 1,
  "title": "Grocery List",
  "content": "Eggs, Milk, Bread",
  "createdAt": "2024-06-11T14:10:00.123"
}

---

## 6️⃣ **Add Validation and Error Examples**

```markdown
## ♻️ Validation & Error Responses

- Sending blank title/content:
  ```json
  {
    "title": "Title is required"
  }

Trying to update or delete a non-existent note:

Json format:

{
  "error": "Note not found"
}

---

## 7️⃣ **Tech Stack, Author & Further Improvements**

```markdown
## 🧰 Tech Stack

- Java 17+
- Spring Boot 3.x
- Spring Data JPA (Hibernate)
- H2 in-memory database
- Jakarta validation

## 👤 Author

Mohamed Afrid Askar Ali  
[GitHub](https://github.com/YOURUSERNAME) | [LinkedIn](https://linkedin.com/in/YOURUSERNAME)

## 🛣️ Possible Next Steps

- Add `updatedAt` timestamp for edits
- Search/filter notes
- Connect to a frontend (React or HTML/JS)
- Deploy API online (Render, Railway)