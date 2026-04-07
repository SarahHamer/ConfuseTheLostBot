# Reinforcement Learning Attack Demo

## Overview
This project is an interactive browser-based demonstration of two reinforcement learning (RL) attack vectors:

- **Reward Hacking** (via high-reward tiles)
- **Adversarial Observation Manipulation** (via fake goals and noise)

The demo visualizes how an RL agent’s behavior changes under these conditions.

---

## How to Run the Demo
Go to https://sarahhamer.github.io/ConfuseTheLostBot/ and have fun. No extra setup is required.

---

## Dependencies
This project has **no external dependencies**.

It runs entirely in the browser using:
- HTML
- CSS
- Vanilla JavaScript

---

## How to Trigger Each Demonstration

### 1. Reward Hacking (Golden Tiles)
- Increase **"Tile Reward"** using the slider.
- Optionally click on the grid to place additional gold tiles.

### 2. Adversarial Observation Manipulation

#### Fake Goal
- Enable **"Fake Goal (Observation Attack)"**
- The agent will pursue an incorrect (fake) goal.

#### Noise
- Increase **"Noise"**
- The perceived goal becomes unstable or random.

---

## Expected Behavior / Output

### Normal Behavior
- The agent moves efficiently toward the **true goal (green tile)** and remains there.

### Reward Hacking
- With high tile reward:
  - The agent prioritizes **gold tiles** over the true goal.
  - It may detour or remain near high-reward tiles.

### Fake Goal Attack
- The agent moves toward the **blue outlined (fake) goal** instead of the true goal.

### Noise
- As noise increases:
  - The agent’s path becomes **erratic or unstable**
  - It may change direction frequently due to incorrect observations.

---

## Interaction Notes
- Click on grid cells to **add/remove reward tiles**
- Use **Step** to move one step at a time
- Use **Run** to observe continuous behavior
- Use **Reset** to restore default state
