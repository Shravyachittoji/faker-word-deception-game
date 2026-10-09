# Faker Word Deception Game

A browser-based multiplayer party game inspired by social deduction games where one player is secretly the Faker, other players know the secret word, and everyone tries to bluff, read clues, and vote the imposter out.

This project is implemented as a single HTML app and is designed for a small group of friends to play together on phones or laptops using shared room codes.

## What it is

Faker is a real-time deception game for 2-12 players.

- One player is randomly chosen as the Faker.
- Everyone else receives a secret word from the active category.
- The Faker only sees the category and must blend in by submitting a misleading clue.
- Players submit one-word clues that hint at the secret word.
- After clues are submitted, the group discusses and votes on who they believe is the Faker.
- If the Faker is caught, the citizens win a point; if the Faker escapes, the Faker earns points.
- If a caught Faker gets a chance to guess the secret word, they can steal extra points.

The game is designed to be fast, social, and playful, making it a good fit for casual online hangouts or in-person party play.

## Features

- Private room creation and room-code joining
- Cross-device multiplayer support
- Avatar selection and nickname support
- Category-based word packs
- Live clue submission and player voting
- Real-time score tracking and leaderboard
- Round reveal screen with Faker and secret word
- Optional Faker guess-to-steal mechanic
- Simple, single-file web app setup

## Project structure

The repository currently contains:

- `faker_word_deception_game.html` — the full game client and game logic
- `README.md` — project documentation

## How it works

1. A host creates a room.
2. Other players join using the 4-character room code.
3. The host picks a category pack such as Animals, Food, Movies, Tech, or Superheroes.
4. A random secret word is selected.
5. One player is assigned as the Faker.
6. Citizens see the secret word; the Faker only sees the category.
7. Each player submits a single-word clue.
8. Everyone reviews the clues and votes for the suspected Faker.
9. Results are revealed, points are awarded, and the next round begins.

## How to use it

### Basic usage

Because this is a frontend app, the main usage flow is:

1. Open `faker_word_deception_game.html` in a browser.
2. Enter a nickname.
3. Create a room, or join a room with a code.
4. Share the room code with friends.
5. Start the game from the lobby when at least 2 players are connected.

### Live multiplayer setup

This app uses Firebase Authentication and Firestore for player rooms, sync, and real-time updates.

The HTML includes a Firebase configuration block that can be customized to match your own Firebase project. If you do not configure Firebase, the app will fall back to placeholder values and will not connect to a working backend for multiplayer play.

To enable real-time multiplayer:

1. Create a Firebase project.
2. Enable Firebase Authentication and Firestore.
3. Replace the demo config in `faker_word_deception_game.html` with your Firebase project configuration.
4. Host the app through a static web server or a Firebase Hosting setup.

### Local preview

You can test the app locally with a simple local web server, for example:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/faker_word_deception_game.html
```

## Notes

- This project is intentionally lightweight and does not use a framework or build system.
- It is best suited for small groups and casual gameplay.
- For real multiplayer sessions, a valid Firebase backend setup is required.

## Example gameplay summary

A typical round looks like this:

- Category: Animals
- Secret word: Elephant
- Faker is assigned
- Citizens submit clues such as "trunk", "gray", or "jungle"
- Faker tries to submit a misleading clue such as "jump"
- Players discuss and vote
- If the Faker is discovered, citizens win
- If the Faker survives, the Faker gains the round points

## License

This project does not currently include an explicit license file. If you plan to share or deploy it publicly, you may want to add a license for clarity.

## Summary

Faker Word Deception Game is a fun browser-based social deduction game that turns a single HTML page into a colorful real-time multiplayer experience. It is easy to run, easy to share, and ideal for casual party-style play with friends.
