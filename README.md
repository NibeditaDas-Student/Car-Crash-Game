# 🚗 Car Crash Game

*A Simple 2D Arcade Car Game using Java Applet & AWT*

---

## 📌 Project Overview

This project is a **2D Car Racing Game** developed using **Java Applet**, **AWT Graphics**, and **Multithreading**.

The player controls a car using the keyboard and must avoid incoming obstacle cars while the game speed increases progressively. The score increases each time an obstacle is successfully avoided.

This project demonstrates fundamental concepts of:

* Java Applet lifecycle
* AWT Graphics rendering
* Keyboard event handling
* Multithreading
* Basic collision detection
* Game loop implementation

---

## 🎮 Gameplay Features

* 🚗 Player-controlled car (Left / Right arrow keys)
* 🚙 Randomly generated obstacle cars
* 🛣️ Moving road animation
* 📈 Progressive difficulty (speed increases with score)
* 🧮 Real-time score tracking
* ❌ Collision detection system
* 🛑 “Game Over” display on crash

---

## 🛠️ Technologies Used

* **Java**
* **Java Applet**
* **AWT (Abstract Window Toolkit)**
* **Multithreading (`Runnable`)**
* **KeyListener (Keyboard Handling)**
* **Graphics API**
* **Random Number Generation**

---

## 🏗️ System Design

### Core Components

| Component     | Description                  |
| ------------- | ---------------------------- |
| `Applet`      | Base class for GUI rendering |
| `Runnable`    | Runs the game loop           |
| `KeyListener` | Handles keyboard input       |
| `Graphics`    | Draws road, cars, and score  |
| `Thread`      | Controls animation timing    |

---

## 🎮 Game Controls

| Key           | Action         |
| ------------- | -------------- |
| ⬅ Left Arrow  | Move car left  |
| ➡ Right Arrow | Move car right |

---

## ⚙️ Game Mechanics

### 1️⃣ Game Loop

The game runs inside a continuous thread:

* Updates positions of:

  * Road strips
  * Obstacle cars
* Checks for collisions
* Adjusts game speed based on score
* Repaints the screen

### 2️⃣ Difficulty Scaling

| Score Range | Game Speed |
| ----------- | ---------- |
| 0 – 2       | Slow       |
| 3 – 4       | Medium     |
| 5 – 6       | Fast       |
| 7+          | Very Fast  |

The `Thread.sleep()` duration decreases as score increases.

---

### 3️⃣ Collision Detection

Collision is detected when:

* The player's car overlaps horizontally with an obstacle
* The obstacle reaches the player’s vertical position

If collision occurs:

* Game displays **"Game Over"**
* Game thread stops

---

## 📂 Project Structure

```bash
CarGame/
│
├── CarGame.java
├── caryellow.png
├── carred.png
└── README.md
```

## ⚠️ Limitations

* Uses deprecated Java Applet technology
* No restart option after Game Over
* No sound effects
* No advanced collision bounding boxes
* No object-oriented separation (single class design)

---

## 👩‍💻 Author

**Nibedita Das**

---

## 📄 License

This project is developed for educational and academic purposes.
Feel free to modify and extend it for learning.

---
* Create a more advanced professional README (for placements)
* Add GitHub badges and portfolio styling
* Convert it into a resume-ready project description

Just tell me your purpose (College / Portfolio / Interview / Resume) 🚀
