# 🎮 Eclipse - Tic Tac Toe
### *Architect Edition*

<div align="center">

![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)
![Platform](https://img.shields.io/badge/platform-Web%20%7C%20Android%20%7C%20iOS-brightgreen.svg)
![License](https://img.shields.io/badge/license-MIT-orange.svg)
![Three.js](https://img.shields.io/badge/Three.js-r128-black.svg)
![Firebase](https://img.shields.io/badge/Firebase-8.10.0-yellow.svg)

**The most beautiful, feature-rich Tic Tac Toe game ever created.**

[Play Now](#-quick-start) • [Features](#-features) • [Screenshots](#-screenshots) • [Installation](#-installation)

---

<img src="https://raw.githubusercontent.com/simple-icons/simple-icons/develop/icons/threedotjs.svg" width="50" alt="Three.js">
&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/simple-icons/simple-icons/develop/icons/firebase.svg" width="50" alt="Firebase">
&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/nicbarker/Tic-Tac-Toe/master/preview.gif" width="200" alt="Preview">

</div>

---

## ✨ Features

### 🎯 Game Modes

| Mode | Description |
|------|-------------|
| 🤖 **VS AI** | Challenge intelligent AI with 3 difficulty levels |
| 🎮 **Local Multiplayer** | Play against a friend on the same device |
| 🌐 **Online Multiplayer** | Real-time battles with players worldwide via Firebase |

### 🧠 AI Difficulty Levels

- **Easy** - Perfect for beginners, makes occasional mistakes
- **Medium** - Balanced gameplay with strategic moves
- **Hard** - Unbeatable minimax algorithm - can you draw against it?

### 🏆 Achievement System (15 Achievements)

<details>
<summary><b>Click to view all achievements</b></summary>

| Achievement | Icon | Description |
|-------------|------|-------------|
| First Blood | 🎯 | Win your first game |
| On Fire | 🔥 | Win 3 games in a row |
| Unstoppable | ⚡ | Win 5 games in a row |
| Legendary | 👑 | Win 10 games in a row |
| AI Slayer | 🤖 | Beat Hard AI |
| Gamer | 🎮 | Play 10 games |
| Veteran | 🏅 | Play 50 games |
| Master | 💎 | Play 100 games |
| Connected | 🌐 | Win an online match |
| Perfect Game | ✨ | Win without opponent getting 2 in a row |
| Speed Demon | ⚡ | Win in under 10 seconds |
| Comeback King | 🔄 | Win after being down 0-2 in a series |
| AI Master | 🧠 | Beat Hard AI 10 times |
| World Traveler | 🌍 | Play 50 online matches |
| Daily Player | 📅 | Play 7 days in a row |

</details>

### 📊 Advanced Statistics

- **Win Rate by Mode** - Track your performance in AI, Local, and Online modes
- **Win Heatmap** - Visualize which board positions you win from most
- **Opening Heatmap** - See your favorite first moves
- **Favorite Opening Analysis** - Discover your most successful strategies
- **Loss Analysis** - Learn from your defeats
- **Daily Streak Tracking** - Stay motivated with daily play tracking
- **Match History** - Review your last 10 games

### 🎨 Customization

| Feature | Options |
|---------|---------|
| **Piece Colors** | 6 colors each for X and O |
| **Board Themes** | Classic, Neon, Wood, Marble |
| **Font Styles** | Modern, Elegant, Retro, Fun |
| **Turn Timer** | Off, 15s, 30s |
| **Match Types** | Endless, Best of 3, Best of 5 |

### 🎪 Special Effects

- 🎉 **Confetti Celebration** - Beautiful particle effects on victory
- ✨ **3D Win Line Animation** - Glowing line shows winning combination
- 💫 **Smooth Piece Animations** - Physics-based piece dropping
- 🎭 **Emote System** - Express yourself with 👋 🤔 👏 during games
- ↩️ **Undo Move** - Take back moves in local games

---

## 🖼️ Screenshots

<div align="center">

| Main Menu | Gameplay | Stats Dashboard |
|:---------:|:--------:|:---------------:|
| 🏠 Elegant cinematic menu | 🎮 3D rendered board | 📊 Detailed analytics |

| Achievements | Settings | Online Match |
|:------------:|:--------:|:------------:|
| 🏆 15 unlockable badges | ⚙️ Full customization | 🌐 Real-time multiplayer |

</div>

---

## 🚀 Quick Start

### Play in Browser
Simply open `index.html` in any modern browser!

```bash
# Clone the repository
git clone https://github.com/nishal21/eclipse-tictactoe.git

# Navigate to the app
cd eclipse-tictactoe/App/www

# Open in browser (macOS)
open index.html

# Or on Linux
xdg-open index.html

# Or on Windows
start index.html
```

### Build as Mobile App (Cordova/Capacitor)

```bash
# Install Cordova
npm install -g cordova

# Create Cordova project
cordova create TicTacToe com.eclipse.tictactoe "Eclipse Tic Tac Toe"

# Copy www folder contents to Cordova www folder
cp -r www/* TicTacToe/www/

# Add platforms
cd TicTacToe
cordova platform add android
cordova platform add ios

# Build
cordova build android
cordova build ios
```

---

## 🛠️ Tech Stack

<div align="center">

| Technology | Purpose |
|:----------:|:-------:|
| ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white) | Structure |
| ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white) | Styling & Animations |
| ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black) | Game Logic |
| ![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=three.js&logoColor=white) | 3D Rendering |
| ![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black) | Real-time Multiplayer |

</div>

### Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                    Eclipse Tic Tac Toe                      │
├─────────────────────────────────────────────────────────────┤
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────────────┐ │
│  │   UI Layer  │  │  3D Engine  │  │  Firebase Backend   │ │
│  │  (HTML/CSS) │  │  (Three.js) │  │  (Auth + Firestore) │ │
│  └──────┬──────┘  └──────┬──────┘  └──────────┬──────────┘ │
│         │                │                     │            │
│         └────────────────┴─────────────────────┘            │
│                          │                                  │
│                   ┌──────┴──────┐                          │
│                   │  Game Core  │                          │
│                   │  (ES6 Class)│                          │
│                   └─────────────┘                          │
│                          │                                  │
│         ┌────────────────┼────────────────┐                │
│         ▼                ▼                ▼                │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐        │
│  │  AI Engine  │  │   Stats     │  │ Achievement │        │
│  │  (Minimax)  │  │  Tracking   │  │   System    │        │
│  └─────────────┘  └─────────────┘  └─────────────┘        │
└─────────────────────────────────────────────────────────────┘
```

---

## 📁 Project Structure

```
eclipse-tictactoe/
├── 📄 index.html          # Single-file app (HTML + CSS + JS)
├── 📄 manifest.json       # PWA manifest
├── 🎵 bgm.mp3            # Background music (optional)
└── 📄 README.md          # You are here!
```

---

## ⚙️ Configuration

### Firebase Setup (for Online Mode)

The app comes pre-configured with Firebase. To use your own:

1. Create a Firebase project at [console.firebase.google.com](https://console.firebase.google.com)
2. Enable Anonymous Authentication
3. Create a Firestore database
4. Replace the Firebase config in `index.html`:

```javascript
const firebaseConfig = {
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_PROJECT.firebaseapp.com",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_PROJECT.appspot.com",
    messagingSenderId: "YOUR_SENDER_ID",
    appId: "YOUR_APP_ID"
};
```

### Background Music

Place your audio file as `bgm.mp3` in the same directory. Supports:
- Volume control (0-100%)
- Auto-loop
- Remembers last volume setting

---

## 🎮 How to Play

### Basic Rules
1. Players take turns placing their mark (X or O)
2. First player to get 3 in a row wins (horizontal, vertical, or diagonal)
3. If all 9 squares are filled with no winner, it's a draw

### Controls
- **Click/Tap** - Place your piece
- **Emote Buttons** - Send reactions during online games
- **Undo Button** - Take back last move (local games only)

### Series Mode
- **Best of 3** - First to win 2 games wins the series
- **Best of 5** - First to win 3 games wins the series
- Players alternate who goes first each round

---

## 🏅 Scoring System

| Result | Points |
|--------|--------|
| Win | +1 to wins, streak continues |
| Loss | +1 to losses, streak resets |
| Draw | +1 to draws |

### Streak Bonuses
- 3 wins → "On Fire" achievement 🔥
- 5 wins → "Unstoppable" achievement ⚡
- 10 wins → "Legendary" achievement 👑

---

## 📱 Responsive Design

Fully optimized for all screen sizes:

- 📱 **Mobile** (< 600px) - Touch-optimized interface
- 📱 **Tablet** (600-900px) - Balanced layout
- 💻 **Desktop** (> 900px) - Full experience
- 🖥️ **Large Screens** (> 1200px) - Enhanced visuals
- 📱 **Landscape Mobile** - Adapted for horizontal play

---

## 🔒 Privacy & Data

- **No personal data collected**
- **Anonymous authentication** for online play
- **Local storage only** for stats and settings
- **No tracking or analytics**
- **No ads**

---

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. 🍴 Fork the repository
2. 🌿 Create a feature branch (`git checkout -b feature/amazing`)
3. 💾 Commit changes (`git commit -m 'Add amazing feature'`)
4. 📤 Push to branch (`git push origin feature/amazing`)
5. 🔃 Open a Pull Request

---

## 👨‍💻 Developer

<div align="center">

### Nishal K

📍 Malappuram, Kerala, India

[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/DemonKing.___)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/nishal21)

</div>

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2025 Nishal K

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

---

## 🙏 Acknowledgments

- [Three.js](https://threejs.org/) - Amazing 3D library
- [Firebase](https://firebase.google.com/) - Real-time backend
- [Google Fonts](https://fonts.google.com/) - Beautiful typography
- [Noto Color Emoji](https://fonts.google.com/noto/specimen/Noto+Color+Emoji) - Cross-platform emoji support

---

<div align="center">

### ⭐ Star this repo if you enjoyed the game!

**Made with ❤️ and ☕ in Kerala, India**

![Wave](https://raw.githubusercontent.com/mayhemantt/mayhemantt/Update/svg/Bottom.svg)

</div>
# Eclips-tictactoe
