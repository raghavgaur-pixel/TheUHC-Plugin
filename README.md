# TheUHC

TheUHC is a Minecraft plugin designed to host a controlled Ultra Hardcore (UHC) style survival event. It provides a structured game flow including a pre-game lobby, synchronized countdown, randomized safe spawning, configurable world border mechanics, and elimination-based gameplay.

---

## Overview

The plugin enables a fair and competitive survival experience where:

- All players begin in a controlled lobby environment
- The game starts simultaneously using a countdown system
- Players are distributed randomly across the world
- PvP is enabled manually by the host
- The world border shrinks in phases
- Eliminated players are converted to spectators
- The final surviving player is declared the winner

---

## Requirements

- Paper or Spigot server (1.21+ recommended)
- Java 17 or higher (Java 21 supported)
- Maven (for building the plugin)

---

## Initial Setup

After the first server start:

1. Stop the server
2. Navigate to:
   /plugins/TheUHC/config.yml
3. Configure the required settings

---

## Configuration

### Lobby Settings

lobby:
  world: world
  x: 0
  y: 200
  z: 0

Ensure this location is safe and contains a platform.

---

### Game Settings

game:
  spawn-protection-seconds: 5
  min-distance-between-players: 20

---

### Border Settings

border:
  start-size: 500

---

### Countdown Settings

countdown:
  seconds: 5

---

## Commands

/startgame

/pvp enable
/pvp disable

/border <size>

---

## Game Flow

1. Players join and are sent to the lobby
2. Host initiates the game using /startgame
3. Countdown begins
4. Players are teleported to random safe locations
5. Players gather resources
6. Host enables PvP
7. Border shrinks
8. Eliminated players become spectators
9. Last player alive wins

---

## Author

Developed by Raghav Gaur
