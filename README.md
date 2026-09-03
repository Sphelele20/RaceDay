# RaceDay - Event Management System

## Overview
RaceDay is a full-stack web-based event management system designed for South African road running, walking, and cycling events. This is Part 1 of the Portfolio of Evidence (POE) which focuses on system planning and database design.

## System Roles

### Organizer
- Create, edit, and delete events
- Manage event categories  
- Capture participant results
- View all event enrollments

### Participant
- Create an account
- Browse events
- Enter events by selecting a category
- View their own enrollments
- Track their personal results

## Project Structure

## Documents Included

### 1. Entity Relationship Diagram (ERD)

- **File:** docs/RaceDay_ERD.png
- **Entities:** 7 tables (Roles, Users, Categories, Events, EventCategories, Enrollments, Results)
- **Relationships:** All primary keys, foreign keys, and cardinalities clearly shown
- **Format:** PNG image for easy viewing

### 2. API Endpoint Plan

- **File:** docs/API_Endpoint_Plan.md
- **Endpoints:** Authentication, Users, Events, Categories, Enrollments, Results
- **Includes:** HTTP methods, routes, descriptions, role requirements, request bodies, expected responses
- **Purpose:** Comprehensive planning before any code is written

### 3. SQL Database Script

- **File:** docs/RaceDay_Schema.sql
- **Tables:** 7 tables matching the ERD exactly
- **Constraints:** Primary keys, foreign keys, NOT NULL, UNIQUE, DEFAULT, CHECK
- **Sample Data:** 2 Organizers, 2 Participants, 3 Events, Categories, Enrollments, Results
- **Features:** Indexes, stored procedures, triggers for data integrity

## Database Schema Summary

| Table | Description | Records |
|-------|-------------|---------|
| Roles | User roles (Organizer, Participant) | 2 |
| Users | User accounts | 4 |
| Categories | Event categories | 4 |
| Events | Race events | 3 |
| EventCategories | Junction table (Events to Categories) | 9 |
| Enrollments | Participant event registrations | 4 |
| Results | Participant race results | 3 |

## Setup Instructions

### Prerequisites

- SQL Server Management Studio (SSMS)
- SQL Server (any edition - Express, Developer, or Standard)

### Steps to Set Up Database

1. Clone the repository

```bash
git clone https://github.com/yourusername/RaceDay.git
cd RaceDay
