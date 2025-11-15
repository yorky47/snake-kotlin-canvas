# Kotlin Snake Game

This is a graphical implementation of the classic "Snake" game, built entirely in **Kotlin** and managed with **Gradle**.

The project uses its own game loop and rendering logic (defined in `Game.kt` and `View.kt`) to draw the game state, including graphical assets for the snake and the walls.

## Key Features

-   **Classic Snake Gameplay:** Control a snake to eat food, grow longer, and avoid running into walls or yourself.
-   **Graphical UI:** Renders the game in a window using graphical assets (like `snake.png` and `bricks.png`) instead of a text-based terminal.
-   **Kotlin-based:** The entire project, from build logic (`build.gradle.kts`) to game logic, is written in Kotlin.
-   **Gradle Project:** A self-contained project managed by Gradle, making it easy to build and run.

## Project Structure

-   `src/main/kotlin/Main.kt`: The main entry point that launches the game.
-   `src/main/kotlin/Game.kt`: Contains the core game loop, state management, and update logic.
-   `src/main/kotlin/Snake.kt`: Defines the `Snake` data class, its movement logic, and direction (`HeadDirection`).
-   `src/main/kotlin/Position.kt`: A utility class for handling (x, y) coordinates on the game grid.
-   `src/main/kotlin/View.kt`: Manages the rendering of the game state, drawing the snake, food, and walls to the screen.
-   `src/main/resources/`: Contains image assets like `snake.png` and `bricks.png`.

## Requirements

-   JDK (Java Development Kit)
-   Gradle (The project includes a Gradle wrapper, `gradlew`, so you don't need a separate installation)

## How to Run

1.  **Clone the repository.**
2.  **Make the wrapper executable** (if not already):
    ```bash
    chmod +x ./gradlew
    ```
3.  **Run the game:**
    ```bash
    ./gradlew run
    ```
    Gradle will automatically build the project and start the main function in `Main.kt`.

## How to Build

To just build the project and create a JAR file, run:

```bash
./gradlew build
