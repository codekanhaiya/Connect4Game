# 🎮 Connect 4 Game – JavaFX Desktop Application

A complete JavaFX-based desktop application of the classic **Connect Four** game. This project is designed to demonstrate concepts like FXML integration, menu bars, media handling, game logic, and JavaFX lifecycle with a fun and interactive UI.

---

## 📁 Project Structure

```
Connect4Game/
    |── .idea/
    |
    ├── installer/
    │       ├── icon.ico
    │       └── Connect4Game.jar                # Executable JAR
    ├── out/
    │     ├── artifacts/
    │     └── production/
    ├── src/
    │       ├── connect4GamePackage/
    │       │        ├── game.fxml               # FXML UI layout
    │       │        ├── gameController.java
    │       │        ├── gameMain.java # Main class
    │       │        └── soundHandler.java
    │       ├── icon/
    │       │     ├── img.ico
    │       │     └── img.jpg
    │       ├── META-INF/
    │       │       └── MANIFEST.MF             # Manifest for JAR
    │       └── res/
    │            └── music.wav                  # Background music
    └── Connect4Game.iml                        # IntelliJ module file
```



---

## 🚀 Features

- 🎲 Classic **Connect Four** gameplay.
- 🎨 Dark Mode and Light Mode toggle.
- 🎵 Play/Stop background music.
- 📜 Menu bar with:
  - File → New Game / Reset Game / Exit
  - Help → About Game / About Developer
  - Settings → Music / Theme
- 📂 Resource handling with FXML, WAV, and custom icons.
- 🧠 Educational structure with clean MVC separation.

---

## 📦 Technologies Used

| Tool                         | Version       | Download Link                                                                 |
|------------------------------|---------------|-------------------------------------------------------------------------------|
| Java (JDK)                   | 1.8.0_212      | [Download Java 1.8.0_212 (Oracle)](https://www.oracle.com/java/technologies/javase/javase8-archive-downloads.html) |
| JavaFX                       | Built-in with JDK 8 | *(No separate install needed)*                                                |
| IntelliJ IDEA Community      | 2017.2.7       | [Download IntelliJ 2017.2.7](https://www.jetbrains.com/idea/download/other.html) |

> **Note:** JavaFX is bundled with JDK 8. No additional modules or SDKs are needed.


---

## 🧑‍🏫 How to Run

1. Clone or download this repository.
2. Open the project in **IntelliJ IDEA**.
3. Ensure **Java 1.8** is set as Project SDK.
4. Mark `res/` as a **resources root**:
   - Right-click → `Mark Directory as` → `Resources Root`
5. Run `gameMain.java`.

---

## 🔧 Build Executable JAR (Optional)

1. In IntelliJ:
   - `File` → `Project Structure` → **Artifacts**
   - Click `+` → **JAR** → *From modules with dependencies*
   - Set Main Class: `connect4GamePackage.gameMain`
   - Include:
     - `game.fxml`
     - `img.jpg` (icon)
     - `music.wav`
     - `MANIFEST.MF`
2. Apply → OK → Build → **Build Artifacts** → `Connect4Game.jar`

The final JAR will be in:
```
out/artifacts/Connect4Game_jar/Connect4Game.jar
```


---


## 💬 "About" Dialogs

### Help → About Game

> **How to play?**  
> Connect Four is a two-player game. Players take turns dropping colored discs into a 7-column, 6-row grid. The first to connect four of their own discs horizontally, vertically, or diagonally wins!

---


## 🎮 Game Logic & Menus

- `gameMain.java`: Initializes the JavaFX stage, sets up the UI, menu bar, music, and event handlers.
- `gameController.java`: Handles game logic, board generation, and player interactions.
- `soundHandler.java`: Manages background music playback.
- `game.fxml`: Declarative layout for the UI grid.

---

## 📥 Download

👉 [Download Connect4Game.jar](#)  

---

## 🧠 Learning Points

- JavaFX structure with **FXML + Controller**.
- Resource loading (`Image`, `AudioClip`, `FXML`) using `getClass().getResource(...)`.
- Custom themes and mode switching using color flags.
- Proper use of **menu bars**, `MenuItem`, and UI feedback.
- Packaging a runnable JAR with dependencies and resources.

---

## 📄 License

This project is open for **learning and personal use**.

---

## 👨‍💻 Author

**Kanhaiya Gupta**  
📧 [kanhaiyaguptaksg@gmail.com](mailto:kanhaiyaguptaksg@gmail.com)  
💻 Aspiring Java Developer | Game Enthusiast

[![Website Badge](https://img.shields.io/badge/Visit-Website-blue)](http://officialkanha.epizy.com/)

---

> _"Code. Learn. Build. Repeat."_ 🧠💻🎮
