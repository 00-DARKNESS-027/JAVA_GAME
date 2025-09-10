# JavaGame

2D multiplayer game written in Java, supporting both local and online play (up to 2 players).  
Includes map management, NPCs, items, cutscenes, music, and sound effects.

## Features

- 2D tile-based graphics
- Online multiplayer (2 players, server-client)
- Multiple maps and interactive objects
- NPCs and cutscenes
- Music and sound effects
- Configuration save system

## Requirements

- Java 17 or higher
- Maven

## How to run the game

1. **Clone the repository:**
   ```sh
   git clone https://github.com/your-username/JavaGameFinal.git
   cd JavaGameFinal
   ```

2. **Build the project:**
   ```sh
   mvn clean package
   ```

3. **Start the server (for multiplayer):**
   ```sh
   java -cp target/JavaGameFinal-1.0-SNAPSHOT.jar network.GameServer
   ```
   The server listens on port 8080 by default. You can change the IP/port in the code if needed.

4. **Start the client (player):**
   ```sh
   java -cp target/JavaGameFinal-1.0-SNAPSHOT.jar Main.Main
   ```
   Follow the on-screen instructions to connect locally or online.

## Multiplayer mode

- Only 2 players can be connected at the same time.
- If a player disconnects, the slot is freed and can be used again.
- Player positions are synchronized in real time.

## Contributing

1. Fork the project
2. Create a branch for your feature/fix
3. Submit a pull request

Improvements to graphics, gameplay, networking, bugfixes, and new features are welcome!


**Note:**  
For issues or suggestions, open an issue on GitHub.  
For technical questions, check the comments in the source code.
