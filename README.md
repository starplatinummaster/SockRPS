# Multiplayer Rock-Paper-Scissors Game Using Socket Programming

## Description
This project is a classic game of Rock-Paper-Scissors implemented using socket programming and the TCP protocol. Players can connect to a server and compete in real-time matches over a network connection. The game is designed to handle multiple players simultaneously, showcasing the use of network programming and client-server architecture in a multiplayer gaming environment.

## Features
- Real-time multiplayer gameplay over a network.
- Uses TCP protocol for reliable communication between client and server.
- Handles multiple concurrent connections, allowing multiple players to join and play.
- Simple and intuitive game interface.

## How It Works
1. Players connect to the game server using a client application.
2. Once connected, players can challenge each other to a match of Rock-Paper-Scissors.
3. The server handles all communication and game logic, ensuring fair play and synchronizing the game state between players.
4. The result of each match is sent back to the players in real-time.

## Getting Started

### Prerequisites
- Python 3.x installed on your machine.
- Basic knowledge of socket programming and TCP/IP networking.

### Running the Server
1. Clone this repository to your local machine.
   ```bash
   git clone https://github.com/starplatinummaster/SockRPS.git
   
## Python Files

### 1. `server.py`
- **Establishes a central server** that listens for incoming connections from clients (players).
- **Manages all game logic**, including receiving player moves and determining match outcomes.
- **Sends game results back** to the clients.
- **Handles multiple concurrent connections**, ensuring that multiple players can connect and play simultaneously.
- **Synchronizes the game state** across all connected clients.

### 2. `client.py`
- **Connects players to the game server** by running a separate instance for each player.
- **Sends the player’s moves** to the server.
- **Receives and displays game results** in real-time.
- **Handles user interaction**, allowing players to input their choices.
- **Acts as the interface** between the player and the server, ensuring smooth gameplay.

### 3. `game.py`
- **Encapsulates the core logic** of the Rock-Paper-Scissors game.
- **Written in PyGame**, a Python library used to create games.
- **Creates the game interface** for players.
- **Defines the game rules** and handles decision-making processes.
- **Determines the outcome** of each match based on player inputs.
- **Maintains a clean separation** of game logic, independent of network and server operations.

### 4. `network.py`
- **Manages network communication** between the client and server.
- **Handles sending and receiving data** over the TCP connection.
- **Ensures correct transmission** and receipt of messages by both ends.
- **Abstracts the complexities of socket programming**, allowing seamless communication between components.
- **Facilitates interaction** between `client.py` and `server.py` without managing low-level network details.
