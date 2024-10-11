# Real-Time Chat Application (Java, TCP/IP)

This is a simple multi-user chat application implemented in Java using TCP/IP. The project utilizes Java Sockets to allow multiple clients to communicate in real-time with a central server. The application handles multiple users using threads and supports basic chat functionalities like setting a nickname, broadcasting messages, and quitting the chat.

## Features
- Multi-user chat functionality with a central server.
- Real-time communication using TCP/IP.
- Concurrency handled via Java threading.
- Clients can set and update nicknames.
- Supports message broadcasting to all connected clients.
- Allows clients to quit the chat gracefully.

## How It Works
The application consists of two main components:
1. **Server**: Manages client connections and broadcasts messages to all connected clients.
2. **Client**: Each client connects to the server, sends and receives messages in real-time.

### Flow
1. The server listens on a specified port (1234) and accepts client connections.
2. Each connected client can send messages to the server.
3. The server broadcasts the received message to all connected clients.
4. Clients can also set or change their nickname and gracefully exit the chat.

## Requirements
- Java 8 or later installed.
- Basic knowledge of Java Socket programming.

## How to Use

### 1. Clone the repository
```bash
git clone https://github.com/your-repo/chat-app.git
cd chat-app
```
### 2.Compile the code
```bash
javac Server.java
javac Client.java
```

### 3.Run the Server
```bash
java Client
```
### 4.Run the Client
```bash
java Client
```

### 5.Commands
```bash
/nick new_nickname: Change your nickname.
/quit: Exit the chat.

```
#### Examples
```bash
Enter your nickname: Shekhar
Shekhar has joined the chat!
Shekhar: Hello, everyone!
