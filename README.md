# Notes API – Java & Spring Boot

A robust RESTful API for secure note management, built with Java 17, Spring Boot, and an in-memory H2 database.  
This project demonstrates key backend development skills: CRUD operations, validation, persistence, and API testing.

---

## 🚀 Features

- Create, Read, Update, and Delete notes via RESTful endpoints
- Automatic creation timestamp for every note
- Data validation: Title and content cannot be blank
- Proper error handling for invalid data or missing notes

---

## ⚙️ How to Run

1. Clone the repository:
   ```sh
   git clone https://github.com/mohamedafrid7087/notesapi.git
   cd notesapi


---

## 2. **Add API Endpoints Table Section**

Add below the "How to Run" section:

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

Request:
```json
POST /notes
{
  "title": "Grocery List",
  "content": "Eggs, Milk, Bread"
}


---

## 4. **Add These Final Sections**

**Tech Stack, Author, and Live Demo link (if deployed):**

```markdown
## 🧰 Tech Stack

- Java 17+
- Spring Boot 3.x
- Spring Data JPA (Hibernate)
- H2 in-memory database
- Jakarta validation

## 👤 Author

Mohamed Afrid Askar Ali  
[GitHub](https://github.com/mohamedafrid7087/notesapi)  
[LinkedIn](https://www.linkedin.com/in/mohamedafrid/)

## 🌐 Live Demo

Deployed at: [https://your-railway-app-url.up.railway.app/notes](https://your-railway-app-url.up.railway.app/notes)  
*(Replace with your actual Railway link)*