# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Tic Tac Toe is a single-page web game. The entire application is contained in `tictactoe.html` with inline HTML, CSS, and JavaScript.

## Architecture

**Single File Structure:**
- `tictactoe.html` — Complete game implementation with:
  - Game state: `cells` array (9 elements), `turn` (X/O), `over` flag
  - Win detection: `checkWin()` checks 8 possible lines
  - Game logic: `play()` handles moves, win/draw detection, turn switching
  - UI rendering: `render()` builds the board from state
  - Styling: Gradient background, responsive grid layout, hover effects, win highlighting

**Game Flow:**
- Players alternate X/O turns by clicking cells
- Win is detected immediately after each move
- Draw occurs when board fills with no winner
- New Game button resets all state

## Running the Game

Open `tictactoe.html` in any modern web browser. No build step required.

## Git Workflow

**Commit Regularly:** As you make changes and complete features, commit immediately to git with clean, descriptive messages. Push to GitHub (`https://github.com/anguyen2396/tictactoe`) regularly to ensure all work is backed up and version-controlled.

**Commit Message Format:** Each commit should represent one logical change (e.g., "Add AI opponent", "Fix win detection edge case"). Messages should be clear and explain what was done and why.

**When to Commit:**
- After completing a feature or feature group
- After fixing a bug
- After refactoring a section
- Never go long without committing—commit at the end of each work session

This ensures we never lose work and can always revert to a previous version if needed.
