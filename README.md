# Cinema-Database-Management

This project is a **Cinema Database Management** built for academic purposes. It models the entire data lifecycle of a cinema including movie listings, screenings, ticketing, seating, and food ordering using relational database principles.

---

## Submitted To

**Sir Hafeez**  
**Date:** May 12, 2023

---

## Team Members

- Muhammad Uzair Khalid — `0258-BSCS-21`
- Wassam Rafiq — `0288-BSCS-21`

---

## Introduction

This database system is designed to enhance cinema operations by efficiently managing:
- Movie show timings
- Tickets and seating arrangements
- Food ordering services

With multiple screens and show slots, this system boosts user experience and overall business effectiveness.

---

## Main Functional Requirements

- A **person** (with at least an ID) can buy tickets for one or more shows.
- Each **ticket** is linked to a unique **seat**.
- A **screen** has a unique type and multiple seats.
- A **movie** can be played on multiple screens at different times.
- **Movies** can belong to multiple **genres**.
- A **person** may or may not order any **food item**.

---

## Verbs (Relationships)

- A `Person` **has a** `Ticket` for a `Show`.
- A `Ticket` **allots a** `Seat`.
- A `Screen` **has many** `Seats`.
- A `Screen` **hosts** a `Show` for a `Movie`.
- A `Movie` **belongs to** one or more `Genres`.
- A `Person` **orders** one or more `Food Items`.

---

## Entities & Attributes

### Nouns & Adjectives

| Entity         | Attributes                                                                 |
|----------------|-----------------------------------------------------------------------------|
| Person         | person\_id, person\_name, person\_mobileno                                  |
| Ticket         | ticket\_id, ticket\_price                                                   |
| Seat           | seat\_id, seat\_name                                                        |
| Screen         | screen\_id, screen\_name                                                    |
| Movie          | movie\_id, movie\_name, movie\_language, movie\_director, movie\_year       |
| Show           | show\_id, start\_time, show\_date                                           |
| Genre          | genre\_id, genre\_name                                                      |
| Food Item      | food\_id, food\_name, unit\_price                                           |
| Order          | order\_id, order\_quantity, total\_price                                    |
| Movie\_Genre   | (Composite Key of Movie ID and Genre ID)                                    |

---

## Diagrams

- **ERD (Entity Relationship Diagram)**
- **Normalized ERD**
- **Relational Model**

---

## Tables Implemented

- Person
- Ticket
- Seat
- Screen
- Movie
- Show
- Genre
- Food Item
- Order
- Movie\_Genre

---

## Sample Data Inserted

Tables have been populated with sample entries for:

- Persons
- Foods
- Orders
- Movies
- Genres
- Shows
- Tickets
- Seats
- Movie\_Genre

---

## Standard SQL Queries

Sample SQL queries implemented in this project include:

1. Display all movies with their genres.
2. List all shows on a specific screen.
3. Display people who have not purchased tickets.
4. Find the most expensive food item ordered.
5. List all available seats for a particular show.
6. Count total tickets sold per movie.
7. Find top 3 most watched movies.
8. Compute total revenue from tickets.
9. List food items ordered by a specific person.
10. Show all bookings for a particular date.
11. Display show timings for a movie.
12. Generate a revenue report per day.

---

## Tech Stack

- **Database Engine:** MS SQL Server
- **Tools Used:** SSMS (SQL Server Management Studio)
- **Modeling:** ERD & Normalization to 3NF

---

## How to Use

1. Create a new SQL database in MS SQL Server.
2. Execute table creation scripts from the provided ERD and relational model.
3. Populate data using the sample records.
4. Run the standard SQL queries for testing and validation.

---

## License

This project is for educational purposes only.

---


