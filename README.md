# Chat Application 📬✨

Welcome to the **Chat Application**! This is a simple, multi-client chat system built in Java ☕ that allows users to connect to a server and exchange messages in real-time. Perfect for learning about socket programming and multi-threaded communication! 🧵💬

## Features 🎉
- **Multi-Client Support** 🤝: Multiple clients can connect to the server and chat simultaneously.
- **Real-Time Messaging** ⚡: Send and receive messages instantly with a user-friendly console interface.
- **User-Friendly** 😊: Easy-to-use prompts for entering server details and usernames.
- **Graceful Exit** 🚪: Type `bye` to disconnect from the chat or `exit` to stop connection attempts.
- **Error Handling** 🛡️: Robust handling for invalid ports, disconnected clients, and message formats.

## Project Structure 📂
```
├── Main.java           # Entry point for the application
├── Client.java         # Handles client-side logic and messaging
├── Server.java         # Manages server connections and client handling
└── CommunicationHandler.java # Processes messages between clients
```

## Getting Started 🏁

### Prerequisites 📋
- **Java JDK** (version 8 or higher) ☕
- A terminal or IDE to run the application 🖥️

### Installation ⚙️
1. **Clone or Download** the project to your local machine 📥:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the project directory 📍:
   ```bash
   cd chat-application
   ```
3. Compile the Java files 🛠️:
   ```bash
   javac org/example/*.java org/example/servers/*.java org/example/clients/*.java
   ```

### Running the Application 🚀
1. **Start the Server** 🌐:
   - Open a terminal and run the `Server` class:
     ```bash
     java org.example.servers.Server
     ```
   - Enter a port number (default is `8888`) or press `ENTER` to use the default.
   - The server will start and wait for client connections.

2. **Start a Client** 👤:
   - Open a new terminal and run the `Client` class:
     ```bash
     java org.example.clients.Client
     ```
   - Enter your username ✍️.
   - Enter the server’s port number (e.g., `8888`) or press `ENTER` for the default.
   - Connect to the server running on `localhost`.

3. **Chat Away!** 💬:
   - Type `Hello!` to see online users 👀.
   - Send messages in the format: `<receiver_name> : <your_message>` (e.g., `Alice : Hi!`).
   - Type `bye` to exit the chat gracefully 🚪.

4. **Run Multiple Clients** 🖥️:
   - Open additional terminals and repeat step 2 to simulate multiple users chatting.

### Example Usage 📜
- **Server Terminal**:
  ```
  Pls, enter a port number for this server or press ENTER to use the default port '8888':
  You can now connect to this server via this port 8888
  Server started!
  Waiting for a client to connect...
  ```

- **Client Terminal (Alice)**:
  ```
  Pls, enter your name here: Alice
  Pls, enter the server port number here or press ENTER to use the default '8888':
  Alice, you're now connected!
  Say Hello! to see your friends online..
  >> This is the message format: <receiver_name> : <your_message>
  ?-> Current logged in users: [Alice]
  ```

- **Sending a Message**:
  ```
  Bob : Hey Bob, what's up?
  >> Your message was sent successfully to Bob
  ```

## Notes 📝
- Ensure the server is running before starting any clients 🕒.
- If you encounter a connection error, verify the port number matches the server’s port 🔌.
- The application uses **TCP** for reliable communication 📡.
- Run multiple clients to test multi-user interactions 🤗.

## Troubleshooting ❗
- **Connection Error**: Check if the server is running and the port is correct.
- **Invalid Port**: Use `8888` or ensure the port is not in use by another application.
- **No Response**: Ensure message format is `<receiver_name> : <message>`.

## Contributing 🤗
Want to add emojis, GUI, or new features? Feel free to fork the project and submit a pull request! 🌟

## License 📜
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Happy Chatting! 🎈💬