# Hotel Booking Application

A full-stack hotel booking web application that enables customers to discover hotels, check room availability, and securely book rooms through a simple and efficient booking process.

---

## Project Overview

The Hotel Booking Application provides a centralized platform where customers can:

* Browse available hotels
* Search hotels based on location and dates
* Filter hotels based on price and amenities
* View hotel and room details
* Check room availability
* Securely book available rooms
* View booking details and booking history
* Cancel bookings

Hotel administrators can manage:

* Hotels
* Room categories
* Rooms
* Pricing
* Amenities
* Hotel bookings

The system is designed with a layered backend architecture and a responsive React frontend.

---

# Tech Stack

## Frontend

* ReactJS
* Vite
* JavaScript / JSX
* React Router
* CSS / Tailwind CSS

## Backend

* Java
* Spring Boot
* Spring Web
* Spring Data JPA
* Spring Security
* JWT Authentication
* Maven

## Database

* PostgreSQL
* Hibernate / JPA

## API & Testing

* REST APIs
* JSON
* Swagger / OpenAPI
* Postman

## Development & Deployment

* Git
* GitHub
* GitHub Actions
* Docker
* Vercel / Render / Railway

#


---

# Authentication APIs

## Register

```http
POST /api/auth/register
```

## Login

```http
POST /api/auth/login
```



---

# Hotel APIs

## Get All Hotels

```http
GET /api/hotels
```

Authentication:

```text
Public
```

---

## Get Hotel

```http
GET /api/hotels/{id}
```

Example:

```http
GET /api/hotels/1
```

---

## Search Hotels

```http
GET /api/hotels/search
```


---

## Create Hotel

```http
POST /api/hotels
```

Authentication:

```text
HOTEL_ADMIN
```


---

## Update Hotel

```http
PUT /api/hotels/{id}
```

---

## Delete Hotel

```http
DELETE /api/hotels/{id}
```

---

# Room APIs

## Get Hotel Rooms

```http
GET /api/hotels/{hotelId}/rooms
```

---

## Get Room

```http
GET /api/rooms/{id}
```

---

## Create Room

```http
POST /api/hotels/{hotelId}/rooms
```

---

## Update Room

```http
PUT /api/rooms/{id}
```

---

## Delete Room

```http
DELETE /api/rooms/{id}
```

---

# Availability API

Check whether a room is available for the selected dates.

```http
GET /api/rooms/availability
```
---

# Booking APIs

## Create Booking

```http
POST /api/bookings
```

Authentication:

```text
Required
```

---

## Get My Bookings

```http
GET /api/bookings/my
```

Authentication:

```text
Required
```

---

## Get Booking Details

```http
GET /api/bookings/{id}
```

Authentication:

```text
Required
```

---

## Cancel Booking

```http
PUT /api/bookings/{id}/cancel
```

Authentication:

```text
Required
```

---

# UI Design


```text
Public Pages
     │
     ├── Home
     ├── Hotel Search
     ├── Hotel Details
     ├── Login
     └── Register
     
Customer Pages
     │
     ├── Booking
     ├── Booking Confirmation
     ├── My Bookings
     └── Booking Details
     
Admin Pages
     │
     ├── Dashboard
     ├── Hotel Management
     ├── Room Category Management
     ├── Room Management
     └── Booking Management
```

---
