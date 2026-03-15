# 🚀 PROG7313 Practical Activity – Adding Firebase Authentication and Per-User Data to Your App

## 📝 Objective

In this activity, you will extend your existing mobile application by integrating Firebase Authentication and ensuring that data is stored separately for each authenticated user.

You may apply this activity to either:
* Digital Detox, or
* MicroTrips

The purpose of this task is to help you move from a single-user local app design toward a more realistic cloud-connected application where each user signs in and only sees their own data.

## Learning Outcomes
You will learn how to:
* Create and configure a Firebase project
* Connect an Android app to Firebase
* Add Firebase Authentication to a Jetpack Compose app
* Register and log in users securely
* Associate stored data with the authenticated user
* Ensure one user cannot see another user’s records
* Structure your app so that authentication and application data remain properly separated

## Overview of the Task

You are required to enhance your existing application by introducing user accounts and per-user data ownership:
* A user must be able to register
* A user must be able to log in
* A user must be able to log out
* The app must recognise the currently authenticated user using the Firebase UUID
* All saved records must belong to that specific user
* When a different user logs in, they must only see their own data

## Scenario Choices

### Option 1: Digital Detox

If you choose Digital Detox, each authenticated user should have their own:
* detox sessions
* streaks
* goals
* preferences
* logs or entries

### Option 2: MicroTrips

If you choose MicroTrips, each authenticated user should have their own:
* saved destinations
* favourites
* notes

## Extension Challenge

If you finish early, add one or more of the following:
* Form validation for email and password
* Loading indicators during login/register
* Friendly error messages
* Persistent login session
* Profile screen showing current user email
* Password reset option