# 🚀 Activity: Build a Community Post-It Board App with Firebase, Supabase, RoomDB, and Theming

## 📝 Objective

In this activity, you will design and build a mobile application called Community Post-It Board.

The app will allow users to:
- register and log in using Firebase Authentication
- create and manage a personal profile
- upload a profile image using Supabase Storage
- view a shared community board of short post-it notes
- react to community notes
- create their own notes and save useful notes from the community board
- cache and store selected app data locally using RoomDB

This activity is designed to help you build a more realistic mobile application architecture where data is split across:
- **Firebase Authentication** for identity
- **Firebase Realtime Database** for shared and user-based cloud data
- **Supabase Storage** for images
- **RoomDB** for local caching and offline support

# 🌍 App Concept

## 💡 Community Post-It Board

This app is a structured, safe, and lightweight shared noticeboard. Instead of open chat or comments, users post short post-it style notes to a shared board.

Examples of note categories:
- 💡 Tip  
- 📚 Learned  
- ⚡ Quick Idea  
- 🧠 Reminder  

Users should be able to react to a note. Keep reactions very limited. For example:
👍 Helpful
❤️ Appreciate

Each user will also have their own personal space where they can:
- view notes they created
- view notes they saved
- manage their profile

# 🎯 Suggested Screens
## 1. Authentication Screen
- register with email/password
- login with email/password

## 2. Community Board
- shared real-time notes
- filter by category

## 3. My Board
- user’s own notes
- saved notes

## 4. Create Note
- short structured input
- category dropdown

## 5. Profile
- edit display name
- upload image (Supabase)
- stored in Firebase

## 6. Theme Support
- light and dark mode

# 🗂 Suggested Firebase DB Structure

users/{uid}/profile  
notes/{noteId}  
userNotes/{uid}/{noteId}  
savedNotes/{uid}/{noteId}