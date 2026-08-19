# Mastermind - Bulls and Cows: a console-based code-breaking game

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)

> 📖 Quick note in Portuguese: You can also read this README in Portuguese. To do so, just access [here](README.pt.md).

## About the project

**Mastermind** is a classic board game where one player, the **CodeMaster**, creates a secret code made of a sequence of colours, and the other player, the **CodeBreaker**, tries to guess it in as few attempts as possible. After each guess, feedback is given as two numbers: how many colours are in the correct position (**a**), and how many are correct but in the wrong position (**b**). This repository implements the classic **Mastermind** game together with its **Bulls and Cows** variant (which uses only two colours, Black and White), both played through the console against a computer-controlled CodeMaster. It was developed for the **Object-Oriented Programming** (Programação Orientada a Objetos) course, by [Guilherme Soares](https://github.com/gcsoares24) && [Vitória Correia](https://github.com/vitoriateixeiracorreia).

### Features

- Two selectable game modes: **MultiColour Mastermind** (six colours: Blue, Red, Yellow, Green, Pink, Orange) and the **Bulls and Cows** binary variant (Black/White), each with its own scoring rules.
- Adjustable difficulty (Easy/Medium/Hard), which sets the secret code length to 4, 5 or 6 pins.
- Feedback given as "a" (correct colour and position) and "b" (correct colour, wrong position) counts after every trial.
- Trial history capped and displayed as the last 10 attempts, alongside the running score.
- Optional hints every 3 rounds that reveal a random colour from the secret code, at the cost of points.
- Tracks the best trial made so far and reveals the secret code when a round ends.
- Object-oriented design: a `Colour` interface implemented by the `BinaryColour` and `MultiColour` enums; a `Code` class (with a `BullsAndCowsCode` subclass overriding the Bulls/Cows scoring rule); a `MastermindGame` interface implemented by the abstract `AbstractMastermindGame`, which is extended by the concrete `BullsAndCows` and `MultiColourMastermindGame` classes.

### Tech stack

- Java
