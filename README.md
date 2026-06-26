# Basic-Programming-Final-Project-student-swing-game-project
 Simple Tic-Tac-Toe Game with Java Swing, Login, and Statistics
## Student Information
Name: Ahza Ahnaf Adrymansyah
Student ID: 5026251123
Class: Q (IUP)
## Project Description
This project is a simple Tic-Tac-Toe game built using Java Swing.
The application includes login, game statistics, and Top 5 scorer
feature.
## Features
- User logs in with their credentials
- Play the tictactoe game 
- Shows wins, loss and draws and record them to the database
- Display the user's statistics int he main menu page
- Displays the leaderboard standings 
## Database
Database used: MySQL 
## How to Run
1. Copy and paste source code to Eclipse IDE (Or download the respitory)
2. Open Eclipse IDE 
3. Import the project folder as a Java project workspace.
4. Open the `Main.java` file.
5. Open XAMPP 
6. Click the green **Run** button to compile and start the application.
7. Click run on `Main.java`
8. Log in using the default testing credentials:
   - **Username:** `player1`
   - **Password:** `pass123`
## Class Explanation
### Main: The central execution entry point of the program. It handles the initial boot configuration and kicks off the `LoginFrame` window.
### DatabaseManager: The data manager of the program. It handles file I/O operations, reads stored rows, initializes default data configurations, and saves/updates player objects inside the text file ecosystem.
### Player: The model class. It represents a singular entity and stores its data such as username, password, wins, losses, draws, and scores from the game.
### PlayerService: The player's logic handler. It acts as the intermediary between the visual frames and the data engine, processing verification rules for logins, account creation checks, and modifying score data dynamically after game outcomes.
### GameLogic: The backbone behind how the TicTacToe game works. It handles the 3x3 game board grid, checks if a player's or computer's move is valid, determines if either the user or computer wins, lose or draws, and handles the automated decision-making for the computer and player’s moves.
### LoginFrame: A login menu that loads up upon starting of the application. It provides text input fields for the username and password, contains a submit action button click, and consults the `PlayerService` to either grant access to the main menu or throw an alert message for incorrect credentials and display it to the user.
### MainMenuFrame: The main navigation GUI of the app. Once a user successfully logs in, this frame dynamically displays a welcome title at the top, then displays current total score, and lifetime match records (wins, losses, and draws). It provides clear button interfaces to launch a new game , view global high scores, or log out back to the login screen.
### GameFrame: This is the interactive game screen. It uses a Swing `GridLayout` to display a visual 3x3 button board representing the Tic-Tac-Toe grid. It captures real-time player mouse clicks to place "X" symbols, updates the header status bar text, updates the layout when the computer plays an "O", and prompts the end-game pop-up messages before sending statistics back to storage.
### StatisticsFrame: A dedicated user profile window on the main menu dedicated to show the user’s current statistics. It translates raw game data into a clean interface layout, allowing players to look at their lifetime stats of the game. 
### TopScorersFrame: This displays the leaderboard of players globally. It constructs a non-editable `JTable` component that prints out rows representing the users in order of points. It handles sorting algorithms internally to order all existing accounts by their total cumulative score, formatting it clearly into ranked places (e.g., 1st, 2nd, 3rd) up to the top 5 competitors.

## Screenshots
<img width="266" height="176" alt="image" src="https://github.com/user-attachments/assets/132eda3a-3683-47e7-91d2-6b7a1ecab292" /> Login Interface

<img width="316" height="358" alt="image" src="https://github.com/user-attachments/assets/6926c25e-0fe0-41af-9067-169d5d80feee" /> Main Menu of the Game

<img width="306" height="351" alt="image" src="https://github.com/user-attachments/assets/259fe601-2657-4b1d-bba1-5b09c9fc940c" /> The game in session

<img width="307" height="352" alt="image" src="https://github.com/user-attachments/assets/ecd78cd4-9ee2-4e27-bdaa-f2de86a26948" /> User Lost, Computer Wins

<img width="301" height="343" alt="image" src="https://github.com/user-attachments/assets/2260a29f-6d4b-42c9-bb3f-cec33990063c" /> User Wins, Computer Loses

<img width="386" height="288" alt="image" src="https://github.com/user-attachments/assets/e3472563-d407-436d-8079-fda279560888" /> Leaderboard Interface








## Video Link
YouTube: https://www.youtube.com/watch?v=7PCKAx_dLto
