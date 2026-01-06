# Full_Stack_MERN_2_Habit_Heatmap_Tracker

## Overview

Habitmap is a habit tracker application built using **Express.js**, **MongoDB**, and **React**.  
It helps users track daily habits, monitor consistency, and analyze progress over time.

---

## Tech Stack

### Frontend
- React

### Backend
- Node.js
- Express.js

### Database
- MongoDB
- Mongoose

---

## Getting Started

### Prerequisites
- Node.js
- MongoDB

---

## Installation

### Step 1: Clone the Repository
```bash
git clone https://github.com/Harshita-Verma09/Full_Stack_MERN_2_Habit_Heatmap_Tracker.git

```
## Usage

### Features
- User authentication
- Create and track habits
- Daily habit logging
- View progress and consistency

---

## MongoDB Schema Design

### User Schema
- username
- email
- password

### Habit Schema
- name
- createdAt

### HabitLog Schema
- name
- date
- taskCompleted
- totalTask
- status

---

## Difficulty 1: Why `date` is Stored as Date Type Instead of String

### Problem
Initially, there was confusion about storing the `date` field as a string or as a `Date` type in MongoDB.

### Solution
The `date` field is stored as a **Date** type because:

- MongoDB supports powerful date-based queries
- Sorting and filtering by date becomes easier
- Aggregation pipelines work efficiently with `Date`
- Avoids manual date parsing and formatting issues
- Helps in future analytics (weekly/monthly reports)

Using `Date` improves **performance, scalability, and data accuracy**.
```


