# Screenshot

## Output UI

| Keterangan | Screenshot |
|------------|------------|
| Tampilan UI di localhost | <img src="https://github.com/user-attachments/assets/0438eb4c-1b13-42d1-a97c-7febf7561c97" width="800"/> |

---

# Documentation: User API Spec

## Create User

Endpoint : POST /api/users

Request Body :

```json
{
  "name": "Nopal",
  "age": 21
}
```

Response Body (Success, 201 Created) :

```json
{
  "status": "success",
  "data": {
    "id": "c32f39d6-1b1a-44b8-b6f9-0e6ef10ea5ad",
    "name": "Nopal",
    "age": 21
  }
}
```

---

## Get All Users

Endpoint : GET /api/users

Response Body (Success, 200 OK) :

```json
{
  "status": "success",
  "data": [
    {
      "id": "89b32b44-eea5-4c22-9dfd-54d19be9197c",
      "name": "Naufal Muhammad Daffa",
      "age": 22
    }
  ]
}
```

---

## Get User By ID

Endpoint : GET /api/users/{id}

Example :  
GET /api/users/89b32b44-eea5-4c22-9dfd-54d19be9197c

Response Body (Success, 200 OK) :

```json
{
  "status": "success",
  "data": {
    "id": "89b32b44-eea5-4c22-9dfd-54d19be9197c",
    "name": "Naufal Muhammad Daffa",
    "age": 22
  }
}
```

---

## Update User

Endpoint : PUT /api/users/{id}

Example :  
PUT /api/users/c32f39d6-1b1a-44b8-b6f9-0e6ef10ea5ad

Request Body :

```json
{
  "name": "Daffa",
  "age": 22
}
```

Response Body (Success, 200 OK) :

```json
{
  "status": "success",
  "data": {
    "id": "c32f39d6-1b1a-44b8-b6f9-0e6ef10ea5ad",
    "name": "Daffa",
    "age": 22
  }
}
```

---

## Delete User

Endpoint : DELETE /api/users/{id}

Example :  
DELETE /api/users/c32f39d6-1b1a-44b8-b6f9-0e6ef10ea5ad

Response Body (Success, 200 OK) :

```json
{
  "status": "success delete user with id c32f39d6-1b1a-44b8-b6f9-0e6ef10ea5ad"
}
```
