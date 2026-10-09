# 🎭 Faker Word Deception Game

<p align="center">
  <img src="https://img.shields.io/badge/HTML-100%25-orange?style=for-the-badge&logo=html5" alt="HTML 100%" />
  <img src="https://img.shields.io/badge/Players-2--12-blue?style=for-the-badge" alt="2-12 players" />
  <img src="https://img.shields.io/badge/Mode-Party%20Game-purple?style=for-the-badge" alt="Party game" />
  <img src="https://img.shields.io/badge/Setup-Single%20File-green?style=for-the-badge" alt="Single file" />
</p>

A fast, social, browser-based deception game inspired by bluffing party classics. One player is secretly the Faker, everyone else knows the secret word, and the group tries to outsmart each other with clues, accusations, and clever lies.

This project is designed to run as a lightweight single-page web app so friends can jump in quickly on phones, tablets, or laptops.

## ✨ Game at a glance

<div align="center">
  <img src="https://raw.githubusercontent.com/Shravyachittoji/faker-word-deception-game/main/preview.png" alt="Game preview placeholder" width="800" />
</div>

> If you want to add a real screenshot later, drop it into the repo as `preview.png` and this card will automatically display it.

### 🧠 Round flow

```text
Secret word: ELEPHANT
             │
             ├─ Citizens see: "ELEPHANT"
             └─ Faker sees only: "Animals"

Players submit clues:
  • trunk
  • gray
  • jungle
  • jump

Then everyone votes:
  • Who is bluffing?
  • Who is lying?
  • Who is actually helping the group?
```

## 🎯 How to play

- One player is randomly chosen as the Faker.
- Everyone else receives a secret word from the active category.
- The Faker only sees the category and must submit a misleading clue.
- Each player gives a one-word clue that could match the secret word.
- The room discusses the clues and votes on the likely impostor.
- If the Faker is caught, the citizens win points.
- If the Faker escapes, the Faker wins points.
- A successful Faker guess can steal extra points.

## 🚀 Features

- Private room creation and room-code joining
- Cross-device multiplayer support
- Nicknames and avatar selection
- Category-based word packs
- Live clue submission and voting
- Real-time score tracking and leaderboard
- Round reveal screen with the Faker and secret word
- Optional Faker guess-to-steal mechanic
- Lightweight single-file app setup

## 🕹️ How it works

1. A host creates a room.
2. Others join with a 4-character room code.
3. The host picks a category such as Animals, Food, Movies, Tech, or Superheroes.
4. A secret word is chosen randomly.
5. One player becomes the Faker.
6. Citizens see the secret word while the Faker only sees the category.
7. Each player submits a one-word clue.
8. Everyone reviews clues and votes for the most suspicious player.
9. Points are awarded and the next round starts.

## 🧩 Project structure

- `faker_word_deception_game.html` — the complete game client and game logic
- `README.md` — project documentation

## 🛠️ Quick start

### Basic usage

Open `faker_word_deception_game.html` in a browser, then:

1. Enter a nickname.
2. Create or join a room.
3. Share the room code with friends.
4. Start the game from the lobby.

### Local preview

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/faker_word_deception_game.html
```

### Firebase multiplayer setup

This app uses Firebase Authentication and Firestore for room sync and real-time updates.

To enable multiplayer:

1. Create a Firebase project.
2. Enable Authentication and Firestore.
3. Replace the demo config inside `faker_word_deception_game.html` with your own Firebase project settings.
4. Host the app via a static web server or Firebase Hosting.

## 🌈 Why it feels fun

```text
⚡ Fast rounds
🎭 Bluffing and suspicion
🧠 Word association chaos
🤝 Shared party energy
```

The game is intentionally lightweight, easy to run, and designed for casual social play with small groups.

## 📝 Notes

- This project is built as a single HTML page with no framework.
- It is best suited for casual, in-person, or online hangouts.
- Real multiplayer requires a valid Firebase backend setup.

## 🏆 Example gameplay summary

```text
Category: Animals
Secret word: Elephant
Faker: assigned
Citizens clue: trunk, gray, jungle
Faker clue: jump
Discussion: who is bluffing?
Outcome: citizens win if they catch the faker
```

## 📜 License

This project does not currently include an explicit license file. If you plan to share or deploy it publicly, consider adding a license for clarity.

## ✅ Summary

Faker Word Deception Game turns a single browser page into a lively, social deduction experience packed with bluffing, guessing, and chaos. It is easy to run, easy to share, and ideal for quick rounds with friends.

<p align="center">
  <sub>Built for laughs, suspicion, and a little bit of strategy.</sub>
</p>
