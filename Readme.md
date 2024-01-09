# Ticket Booking System Database Assignment

## Introduction

This repository contains the solution for the Ticket Booking System Database Assignment. The assignment focuses on designing a relational database for a ticket booking system, where users can book tickets for movies at different theaters.

## Database Structure

The database is designed to adhere to the basic principles.The main entities involved in the system are User, Movie, Theatre, Show, and Booking. Each entity has been carefully structured to eliminate redundancy and ensure data integrity.

### Tables

1. **User Table**
   - UserID (Primary Key)
   - UserEmail (Unique)
   - phone (Unique)
   - UserName
   - password
   - date_of_birth
   - registration_date

2. **Movie Table**
   - MovieID (Primary Key)
   - MovieName

3. **Theatre Table**
   - TheatreID (Primary Key)
   - TheatreName

4. **Show Table**
   - ShowID (Primary Key)
   - TheatreID (Foreign Key referencing Theatre)
   - MovieID (Foreign Key referencing Movie)
   - ShowDate
   - ShowTime

5. **Booking Table**
   - BookingID (Primary Key)
   - UserID (Foreign Key referencing User)
   - ShowID (Foreign Key referencing Show)
   - BookingDate
