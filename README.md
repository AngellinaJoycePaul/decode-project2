# Project 2: Database Integration (CRUD)
**Decode Labs Backend Development Internship**
Built by: Angellina Joyce Paul

## 📌 About
A REST API with full CRUD operations connected to a SQLite database using SQLAlchemy ORM.

## 🛠️ Tech Stack
- Python 3.14
- FastAPI
- SQLAlchemy
- SQLite
- Pydantic

## 🚀 How to Run
1. Create virtual environment
   python -m venv venv
   venv\Scripts\activate

2. Install dependencies
   pip install fastapi uvicorn sqlalchemy pydantic[email]

3. Run the server
   uvicorn main:app --reload

4. Open docs at
   http://127.0.0.1:8000/docs

## 📡 API Routes
| Method | Route | Description | Status Code |
|--------|-------|-------------|-------------|
| POST | /users | Create new user | 201 / 400 / 409 |
| GET | /users | Get all users | 200 |
| GET | /users/{id} | Get single user | 200 / 404 |
| PATCH | /users/{id} | Update user | 200 / 404 / 409 |
| DELETE | /users/{id} | Delete user | 204 / 404 |

## 📸 Screenshots
### Swagger UI Homepage
![Swagger UI](screenshots/1_swagger_ui.PNG)

### POST /users — 201 Created
![201 Created](screenshots/2_post_users1.PNG)

### POST /users — 409 Conflict
![409 Conflict](screenshots/3_post_users2.PNG)

### GET /users — 200 OK
![200 OK](screenshots/4_get_users.PNG)

### GET /users/99 — 404 Not Found
![404 Not Found](screenshots/5_get_users_id.PNG)

### POST /users — 400 Bad Request
![400 Bad Request](screenshots/6_post_users3.PNG)

### PATCH /users/1 — 200 Updated
![200 Updated](screenshots/7_patch.PNG)

### DELETE /users/1 — 204 No Content
![204 Deleted](screenshots/8_delete.PNG)