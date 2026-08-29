# DuoPlay — 2 Player Online Games

A GitHub Pages-friendly multiplayer game site using Firebase Realtime Database + anonymous auth.

## Included games

1. Tic-Tac-Toe
2. Connect 4
3. Rock Paper Scissors
4. Spy vs Spy
5. Mini Battle Arena
6. Battleship
7. Quiz Duel
8. 2D Racing
9. Bow & Arrow Duel
10. Bomb Arena
11. Word Battle
12. Castle Defense
13. Hidden Number

## Firebase setup

1. Create a Firebase project.
2. Add a Web App and copy its config into `firebase-config.js`.
3. Enable **Authentication → Sign-in method → Anonymous**.
4. Create a **Realtime Database**.
5. For a private prototype, use Firebase's development rules while testing. Before making the site public, replace them with authenticated/validated rules so players cannot overwrite arbitrary rooms.
6. Upload the files to GitHub.
7. Enable GitHub Pages from the repository's Pages settings.

The Firebase web config is not a password; database rules and authentication are what protect your data.

## Adding another game

Add one entry to the `games` object, create its initial state in `fresh()`, add a renderer to `RENDER`, and add its move function. The same room system and Firebase backend can be reused.


## Important
This package includes the Firebase config for the DuoPlay project supplied during setup. Before testing, enable Anonymous Authentication and create the Realtime Database. If Create Room fails, the page now shows the Firebase error code instead of silently failing.
