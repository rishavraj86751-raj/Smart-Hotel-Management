# Smart Hotel Management System

Database Project, Vellore Institute of Technology (VIT)
Under the guidance of **Nageshwar Rao Ragi

## About
A database-driven hotel management system that handles guests, rooms,
reservations, check-in/check-out, services, payments, staff and feedback.
Business rules (double-booking prevention, automatic room status,
service pricing, billing, audit log) are enforced inside the database
using constraints, triggers and views.

## Features
- 12 tables in 3NF, 12 foreign keys
- 8 triggers and 3 views
- Double-booking prevention (API check + database trigger)
- Automatic billing: nights x room price + services - payments
- Front desk: check-in, add services, check-out with final bill
- 10 management reports (JOIN, GROUP BY/HAVING, RANK(), self join, subquery)
- Audit log of every reservation status change

## Tech Stack
- Front end: HTML, CSS, JavaScript
- Back end: Python, Flask (REST API)
- Database: SQLite (schema is portable to Oracle)

## How to Run
```
git clone https://github.com/rishavraj86751-raj/Smart-Hotel-Management.git
cd Smart-Hotel-Management
pip install -r requirements.txt
python app.py
```
Open http://localhost:5000 in your browser.
The project report is at http://localhost:5000/report.html

Delete `hotel.db` to reset the sample data.

## Run the tests
Start the app, then in another terminal:
```
python test_all.py
```
Expected result: 36 passed, 0 failed.

## Project Files
| File | Purpose |
|---|---|
| app.py | Flask API, database schema, triggers, views, sample data |
| static/ | Web app (index.html) and project report (report.html) |
| schema.sql | Full SQL: tables, indexes, views, triggers |
| test_all.py | 36 automated checks |
| DEMO_SCRIPT.md | Demo flow and viva questions |

## Live Demo
Add your link here after deploying (Render).
