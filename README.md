# Single-Threaded Socket-Based Web Server (Java)

## 📌 Overview

This project is a basic **single-threaded client-server application** built using Java sockets. It demonstrates how low-level network communication works using the TCP protocol.

The server listens for incoming client connections, processes requests, and sends responses back over a socket connection.

---

## ⚙️ How It Works

1. The server starts and listens on a specific port (`8010`)
2. A client connects to the server using the same port
3. The client sends a message to the server
4. The server reads the message and prints it
5. The server sends a response back to the client
6. The connection is closed

---

## 🧱 Tech Stack

* Java
* Socket Programming (TCP)
* Input/Output Streams

---

## 📂 Project Structure

```
.
├── Client.java
├── Server.java
├── .gitignore
```

---

## ▶️ How to Run

### 1. Compile the files

```
javac Server.java
javac Client.java
```

### 2. Run the server

```
java Server
```

### 3. Run the client (in a new terminal)

```
java Client
```

---

## 💡 Sample Output

### Server:

```
Server is listening on port 8010
Connection accepted from /127.0.0.1
Hello from the client.
```

### Client:

```
Response from the server is :Hello from the server
```

---

## 🧠 Key Concepts Learned

* Working with `ServerSocket` and `Socket`
* Establishing TCP connections
* Reading and writing data using streams
* Understanding request-response communication
* Handling connections sequentially (single-threaded model)

---

## ⚠️ Limitations

* Handles only one client at a time (blocking I/O)
* No concurrency (single-threaded)
* No HTTP protocol parsing (raw message exchange)

---

## 🚀 Possible Improvements

* Add multi-threading to handle multiple clients
* Implement basic HTTP request parsing
* Serve static HTML files
* Add logging for requests and responses
* Introduce timeout and error handling improvements

---

## 🎯 Learning Outcome

This project helped build a foundational understanding of how servers work at a low level.

---

