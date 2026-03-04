# 🎮 Advanced Tic Tac Toe Variations Engine (C++ OOP Framework)

A modular and extensible board game engine built in C++ using Object-Oriented Programming principles.
This project implements 13 Tic Tac Toe variations using a reusable game framework based on templates, inheritance, and polymorphism.

Developed as part of CS213 – Object-Oriented Programming at Cairo University.

## 📌 Project Overview

This project demonstrates how to design a generic board game framework and extend it to implement multiple game variations without modifying the core engine.

The system is built around:

A reusable Board<T> abstraction

A flexible GameManager<T> controller

Support for multiple board types and rule systems

Human vs Human and Human vs Computer gameplay

AI players (for selected games)

The architecture follows the Open/Closed Principle:

The framework is closed for modification but open for extension.

## 🏗 Architecture

The project is built around a generic framework containing the following core components:

#### 🔹 Board<T> (Abstract)

Represents the game board.
Responsible for:

Storing the grid

Validating moves

Checking win/draw/lose conditions

Each game variation inherits from this class and implements its own rules.

#### 🔹 Player<T>

Represents a player (Human or Computer).
Stores:

Name

Symbol

Player type

Reference to board

Custom AI players extend this class.

#### 🔹 Move<T>

Encapsulates a single move:

Position (x, y)

Symbol or value placed

#### 🔹 UI<T> (Abstract)

Handles:

Displaying the board

Receiving input

Showing game messages

Each game provides its own UI implementation.

#### 🔹 GameManager<T>

Controls:

Turn switching

Game loop execution

Win/draw detection

Board updates

This class remains unchanged and can run any game built on the framework.

## 🎮 Implemented Game Variations
#### 🧍 Individual Games

SUS

Four-in-a-row

5×5 Tic Tac Toe

Word Tic Tac Toe

Misère Tic Tac Toe

Diamond Tic Tac Toe

4×4 Moving Tic Tac Toe

Pyramid Tic Tac Toe

#### 👥 Group Games

Numerical Tic Tac Toe

Obstacles Tic Tac Toe

Infinity Tic Tac Toe

Ultimate Tic Tac Toe

Memory Tic Tac Toe

## 🧠 OOP Principles Applied

This project demonstrates the four core OOP principles:

#### Encapsulation
Board state and logic are protected inside classes.

#### Abstraction
Abstract base classes (Board, UI) define interfaces.

#### Inheritance
Each game extends the base framework.

#### Polymorphism
GameManager interacts with games through base class pointers.

## 🎥 Demo
A demonstration video showcasing selected games is available here (in arabic):
https://drive.google.com/file/d/1zqwxcmRrkVnIJGcJ4BTx25DI7mrxSYQR/view

