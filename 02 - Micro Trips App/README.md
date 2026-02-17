# 🚀 Micro Trips App

## 📝 Objective
You will build a real-world, user-friendly travel discovery app which you can name on your own.
The app helps users discover hidden gems in South Africa using image cards, view travel cost breakdowns, save favourites, and open each location in Google Maps — all using local JSON data (no RoomDB, no FirebaseDB, no Auth yet).

## 💡 App Concept
Allow users to discover South African “micro-trips” (short outings) with:
* Aesthetic card UI with images
* Detail pages with budget breakdown (transport, food, entry, misc)
* Saved screen (bookmarked gems)
* Settings screen (dark mode, dynamic color, large text, budget badges)
* Navigation drawer + TopAppBar
* Open in Google Maps intent per spot
* All content loaded from local JSON + local images

## 📦 Constraints
You app must incorporate:
* TopAppBar + Navigation Drawer
* Explore screen with image cards
* Details screen with (image header + info + budget breakdown)
* Google Maps intent (geo: query)
* Savings of spots, and viewing saved spots
* Settings screen
* JSON parsing from assets
* Image loading from assets
* Theme files: Color.kt, Theme.kt, Type.kt

## 🚫 Not needed, for now
* RoomDB
* Firebase
* Authentication
* Network calls / APIs

## 📚 Resources to Read Before You Start
Research/Revise these aspects as you plan your work:
* 📜 Jetpack Compose Basics (Layouts + State)
* 🧭 Navigation Compose (NavHost + routes)
* 🖼️ Coil Compose (image loading)
* 📦 Kotlin Serialization (JSON parsing)
* ⚙️ DataStore Preferences (local settings storage)
* 🎨 Material 3 Theming (ColorScheme + Typography)

## 🏗️ Deliverables
You must submit a GitHub repo containing:
* Code
    * All Compose screens + navigation
    * Drawer + TopAppBar
    * JSON loading + parsing
    * Settings persistence (local)
* Assets
    * assets/data/gems.json
    * assets/data/categories.json
    * assets/data/provinces.json
    * assets/images/ (at least 10 images)
    * App Icon
    * Splash screen
* Documentation
    * A README.md including:
        * App name + tagline
        * Screenshots (or emulator screenshots)
        * Feature list
        * How to run
        * Known limitations
