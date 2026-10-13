# Memory Game

A desktop memory-matching game built with Java Swing. Test your memory by uncovering cards, finding all six matching pairs, and improving your accuracy.

## About the Game

The game features a blue-themed desktop interface with a large title banner, a 3 x 4 card grid, and a side panel for game statistics and controls. Twelve cards are shuffled into six pairs at the start of each round.

Choose two cards to reveal their icons. Matching cards stay face up; non-matching cards are turned face down after a short pause. The statistics panel tracks moves, misses, and accuracy throughout the round.

## Features

- Single-player memory matching on a desktop
- 12 cards with six pairs of icons, shuffled for each round
- Matching cards remain revealed; unmatched cards are hidden again
- Live moves, misses, and accuracy statistics
- Victory dialog with the final round statistics
- **Reset Game** shuffles a new round and resets the counters
- **Exit Game** closes the application
- Centered Swing window with Nimbus look and feel when available

## How to Play

1. Click any card in the grid to reveal its icon.
2. Click a second card to try to find its matching pair.
3. Matching cards remain visible. If they do not match, both are hidden again after a short pause.
4. Find all six pairs to complete the round and view your final statistics.
5. Choose **Reset Game** to start over with newly shuffled cards, or **Exit Game** to close the game.

**Moves** count attempts to reveal a pair. **Misses** count attempts where the two cards do not match. **Accuracy** is calculated from successful matching attempts as a percentage of total moves.

## Requirements

- Java Development Kit (JDK) 25 or later
- Apache Maven
- Apache NetBeans with Java and Maven support (optional, for the IDE workflow)

The project uses the `AbsoluteLayout` library bundled in the repository's `lib/` directory and declared in `pom.xml`.

## Build and Run

### From the command line

In the project root, build the project:

```bash
mvn clean package
```

Launch the game with Maven:

```bash
mvn exec:java -Dexec.mainClass=com.mycompany.memorygame.game
```

### In Apache NetBeans

1. Choose **File > Open Project** and open the folder containing `pom.xml`.
2. Allow Maven to load the project and dependencies.
3. Open `src/main/java/com/mycompany/memorygame/game.java`.
4. Right-click the file and select **Run File**.

A graphical desktop environment is required to run the game.

## Project Structure

```text
.
├── lib/
│   └── unknown/binary/AbsoluteLayout/SNAPSHOT/
│       └── AbsoluteLayout-SNAPSHOT.jar
├── pom.xml
└── src/main/
    ├── java/com/mycompany/memorygame/
    │   ├── game.form
    │   ├── game.java
    │   └── icons/
    └── resources/com/mycompany/memorygame/icons/
```

| Path | Description |
| --- | --- |
| `src/main/java/com/mycompany/memorygame/game.java` | Application entry point, Swing interface, and game logic |
| `src/main/java/com/mycompany/memorygame/game.form` | NetBeans GUI form definition |
| `src/main/java/com/mycompany/memorygame/icons/` | Game icon assets |
| `src/main/resources/com/mycompany/memorygame/icons/` | Icon resources packaged with the application |
| `lib/unknown/binary/AbsoluteLayout/SNAPSHOT/AbsoluteLayout-SNAPSHOT.jar` | Bundled AbsoluteLayout dependency |
| `pom.xml` | Maven project configuration and dependencies |

## Technology

- Java 25
- Java Swing
- Apache NetBeans
- Apache Maven
- AbsoluteLayout

## License

This project is available under the MIT License. Free to use, modify, and distribute with proper attribution.

## Author

**Malik Lateef**  
Software Engineering Student  
Lahore, Pakistan  
Email: [imaliklateef@gmail.com](mailto:imaliklateef@gmail.com)

> An academic portfolio project demonstrating Java Swing, event-driven interfaces, and memory-game logic.
