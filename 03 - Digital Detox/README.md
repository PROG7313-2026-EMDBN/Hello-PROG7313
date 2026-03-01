# 🚀 PROG7313 Practical Activity – Digital Detox Tracker (Room + Compose)

## 📝 Objective

In this activity you will build a Digital Detox Tracker Android app using Jetpack Compose and Room (RoomDB).

You will learn how to:
* Store time-based sessions in Room
* Use DAO queries to produce useful stats (not boring CRUD)
* Use Navigation + ViewModel + StateFlow
* Build a simple dashboard with a live timer
* Build a History list with Edit + Delete
* Calculate streaks from saved session history

## ✅ App Concept
What the user can do
* Start a session (Focus / Screen-free / Phone-free / Study / Deep Work)
* End a session (or mark as interrupted)
* Add/edit notes for a completed session
* View:
    * Current running session timer (live)
    * Weekly total minutes
    * Current streak + best streak
    * History list (edit/delete)

## 🧱 Core Features You Must Build

### ✅ Screen 1: Home (Dashboard)

Must include:
* App title
* Category selector
* Big Start button when no session is running
* When running:
    * Live timer HH:MM:SS
    * End button
    * Interrupted button
* Quick stats:
    * Week minutes
    * Current streak
    * Best streak
    * Button to open History
### ✅ Screen 2: History

Must include:
* List all sessions newest-first
* Each row shows:
    * Category
    * Duration
    * Notes (if any)
* “Interrupted” label if true
* Tap row → open Edit screen
* Delete button (or long press)

### ✅ Screen 3: Edit Session

Must include:
* Category + status (Completed/Running)
* Notes field (to edit)
* Save button

## 🗃️ Database Requirements (RoomDB)
### ✅ Entity: DetoxSession
Store one “time block”.

Minimum fields:
* id (auto)
* startTime (epoch millis)
* endTime (epoch millis, nullable when running)
* category (string)
* notes (string)
* wasInterrupted (boolean)
* createdAt (epoch millis)

## 🧠 SQL Queries You Must Implement (DAO)

You must include these DAO queries:
1. History (all sessions)
    * Sorted newest-first
2. Running session
    * Find the session where endTime IS NULL
3. Weekly total minutes
    * Use SUM(endTime - startTime) for completed sessions
    * Use week start/end epoch millis range
4. Streak support
    * You must load history and calculate:
        * Current streak (consecutive days with at least 1 completed session)
        * Best streak (longest chain)