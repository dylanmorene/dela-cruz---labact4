# Lab SQL Queries API

**Author:** Dylan Morene Dela Cruz

## Description
A Node.js/Express API project to explore SQL queries with MySQL. This project helps you learn and test database operations such as joins, unions, full outer join emulation, and subqueries using Postman.

## Tech Stack
- MySQL
- SQL
- Node.js / Express
- Postman

## Features
- Retrieve latest login per user
- View referral relationships
- Generate all possible user-role combinations
- Emulate full outer joins
- List roles with their assigned users (including empty roles)
- Fetch users with profile information
- List users with assigned roles

## Installation
1. Set up a local or cloud MySQL database.
2. Import SQL scripts from the project.
3. Install Node.js dependencies:
   ```bash
   npm install
   
API Endpoints
Endpoint	Method	Description
/api/reports/users-with-roles	GET	List all users with their assigned roles (INNER JOIN).
/api/reports/users-with-profiles	GET	List all users with profiles, including users without profiles (LEFT JOIN).
/api/reports/roles-right-join	GET	List roles with assigned users, including roles with no users (RIGHT JOIN).
/api/reports/profiles-full-outer	GET	Emulate full outer join for users and profiles (LEFT + RIGHT JOIN with UNION).
/api/reports/user-role-combos	GET	Generate all possible user-role combinations (CROSS JOIN).
/api/reports/referrals	GET	Show referral relationships (SELF JOIN / INNER JOIN).
/api/reports/latest-login	GET	Retrieve each user’s most recent login IP and timestamp (LEFT JOIN + subquery).
Query Types Overview

INNER JOIN: Users with roles

LEFT JOIN: Users with profile info

RIGHT JOIN: Roles with users (including empty roles)

LEFT + RIGHT JOIN UNION: Full outer join emulation

CROSS JOIN: All user-role combinations

SELF JOIN (INNER JOIN): Referral relationships

LEFT JOIN + Subquery: Latest login per user

Usage

Run API endpoints to explore query results.

Test outputs in Postman.

Learn SQL joins, unions, and backend data workflows.
