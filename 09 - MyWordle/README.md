# Activity: Build a Wordle-Style Game in Kotlin Using Jetpack Compose Canvas

## Objective

In this activity, you will design and build a Kotlin Android game inspired by Wordle.

The purpose of this activity is to give you practical experience with custom drawing in modern Android development.In Jetpack Compose, we can harness the `Canvas` composable for animations and drawing.

You will use Kotlin and Jetpack Compose to create a custom game board, animate user feedback, calculate points, and unlock badges based on player performance.

## Activity Description

You are required to build a mobile game similar to Wordle.

The player must guess a hidden five-letter word. After each guess, the game must show feedback for each letter.

Each letter should be marked as one of the following:
- correct letter in the correct position
- correct letter in the wrong position
- letter not found in the hidden word
- empty tile

Your game must not only work logically. It must also feel like a small playable game. This means it must include animations, points, badges, and clear visual feedback.

The main focus of this activity is to use Jetpack Compose `Canvas` to draw the game board instead of building the entire board only with standard layout components.

## Grouping Options
You may complete this activity in one of the following ways.
* You complete the full game yourself.
* Work in pairs on the same codebase.
* Work in a group of three students.

## Recommended Technology

You may use the following technologies:
```text
Kotlin
Jetpack Compose
Compose Canvas
Compose State
Compose Animations
ViewModel
```

You are not required to use Firebase, RoomDB, Supabase, APIs, or external databases for this version.

The focus is on:
- game logic
- custom drawing
- animation
- state management
- gamification

## Game Requirements

### 1. Game Board

Create a board with:
- 6 rows
- 5 columns

So:
* Each row represents one guess.
* Each tile must display one letter or remain empty.
* Each tile must also show a visual state:  
    * Empty - No letter has been entered yet
    * Correct - Letter is in the word and in the correct position
    * Present - Letter is in the word but in the wrong position
    * Absent - Letter is not in the word

The board must be drawn using Jetpack Compose `Canvas`.

You may use other Compose components around the board, such as `Column`, `Button`, `TextField`, and `Text`, but the actual board must be drawn with `Canvas`.

### 2. Word Input

Allow the player to enter a five-letter word.


### 3. Word Checking Logic

When the player submits a guess, compare it to the hidden word.

Example:

```text
Hidden word: PLANT
Guess:      PLACE
```

Possible result:

```text
P = correct
L = correct
A = correct
C = absent
E = absent
```

Your game must store the result for each letter so that the board can display the correct feedback.

### 4. Animations

Your game must include at least two animations.

Choose from the following ideas:

- tile flip animation after a guess is submitted
- shake animation for an invalid word
- scale animation when a letter is typed
- colour transition when feedback is revealed
- badge unlock animation
- win celebration animation
- lose screen animation

### 5. Points System

Add a points system to your game.

You may use the scoting system given below:
- Correct word in 1 guess = 100
- Correct word in 2 guesses = 80
- Correct word in 3 guesses = 60
- Correct word in 4 guesses = 40
- Correct word in 5 guesses = 25
- Correct word in 6 guesses = 10
- Invalid guess = -5

You may adjust the values, but your scoring system must be clearly explained in your README.

Your app must display the score on the screen as the user guesses.

### 6. Badges and Achievements

Add at least two badges.

Each badge must have:
- a badge name
- a short description
- an unlock condition
- a visual display in the app

Badges ideas:
* First Win - Player wins for the first correct guess
* No Mistakes - Player wins without invalid guesses
* Quick Thinker - Player solves the word in 3 guesses or fewer
* Comeback Win - Player wins on the final guess

## Planning your time

Use the time given to build a working playable version first, then add polish.
* Hour 1 - Setup and planning
    * Create the Android project, agree on roles, set up the package structure, create the word list, models, and basic screen layout.
* Hour 2 - Game logic
    * Add the hidden word, current guess, submit button, guess history, and word checking logic. The game should be able to accept guesses and store results.
* Hour 3 - Canvas board 
    * Draw the 6 x 5 board using Jetpack Compose Canvas. Display letters and tile states for empty, correct, present, and absent letters.
* Hour 4 - Playable game loop
    * Add win and lose conditions, prevent extra guesses after the game ends, show result messages, and allow the user to restart the game.
* Hour 5 - Gamification and animation
    * Add the points system, at least two badges, and at least two animations such as tile feedback, invalid guess shake, badge reveal, or win animation.
* Hour 6 - Testing, README
    * Test the full game, fix obvious bugs, complete the README with add screenshots.

## README Requirements

Your README must include:
- project name
- group members and roles
- short description of the game
- how to run the app
- game rules
- points system
- badges and unlock conditions
- features completed
- known issues
- screenshots
- references and resources used

## Resources to Consult

You may consult the following resources while building your app.
* Graphics in Compose: https://developer.android.com/develop/ui/compose/graphics/draw/overview
* Animation in Compose: https://developer.android.com/develop/ui/compose/animation/introduction
* State in Jetpack Compose: https://developer.android.com/develop/ui/compose/state
* Kotlin Coroutines on Android: https://developer.android.com/kotlin/coroutines
