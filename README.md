# ENEI-Gest: Event Management Database

## About this project
This repository contains the database project "ENEI-Gest", built entirely with MySQL. It was developed to handle the backend data management for large-scale academic and tech events, such as ENEI. 

The goal was to build a secure, well-structured relational database that connects event organizers, speakers, sponsors, and attendees in one place.

## What it does
* **Ticketing and Payments:** Manages user registrations, tracks different types of tickets, and monitors pending or confirmed payments.
* **Agenda Management:** Organizes the event into days, sessions, and individual lectures, linking each talk to its respective speaker and location.
* **Sponsorships:** Keeps track of corporate sponsors and their financial contributions to specific events.
* **Access Control:** Uses different database user profiles (like content managers and participant managers) so people only access the data they need to do their jobs.

## Under the hood (Technical details)
This project goes beyond basic table creation. It applies several advanced SQL features to automate tasks and improve performance:
* **Views:** Custom virtual tables created to make reading the public agenda and financial summaries much easier.
* **Stored Procedures & Functions:** Custom SQL scripts to handle business logic, such as automatically calculating the total revenue of an event (combining tickets and sponsorships).
* **Triggers:** Automated actions, like automatically updating a user's registration status to "Confirmed" the moment a new payment is inserted into the system.
* **Indexes:** Applied to key columns to ensure the database remains fast and responsive, even if the number of attendees grows significantly.

## Built with
* MySQL 8.0
* EER Modeling (Conceptual, Logical, and Physical design)
