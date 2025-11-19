
# 🚀 Python TCP Chatroom

A simple multithreaded **TCP chatroom application** built using Python’s `socket` and `threading` modules.
This project demonstrates a basic client–server architecture where multiple clients can join the chatroom, choose an alias, send messages, and receive real-time updates from other participants.

---

## 📌 Features

* 🔹 **Multithreaded server** capable of handling multiple clients simultaneously
* 🔹 **Real-time message broadcasting** to all connected users
* 🔹 **Alias-based identification** for clients
* 🔹 **Graceful handling** of client disconnections
* 🔹 Simple and lightweight Python implementation
* 🔹 Runs on localhost (127.0.0.1) using TCP sockets

---

## 🛠️ Tech Stack

* **Python 3**
* `socket` module (for TCP communication)
* `threading` module (for handling concurrent clients)

---

## 📁 Project Structure

```
├── server.py   # Chatroom server code
└── client.py   # Client-side script for connecting to the chatroom
```

---

## ▶️ How to Run

### 1️⃣ Clone the repository

```bash
git clone https://github.com/kavinda2024/python-tcp-chatroom.git
cd into the repository
```

### 2️⃣ Start the Server

Run this from your terminal:

```bash
python server.py
```

### 3️⃣ Start a Client

Open another terminal window and run:

```bash
python client.py
```

Enter an alias when prompted and start chatting!

### 4️⃣ Connect multiple clients

Open more terminals and run `client.py` again to simulate multiple users.

---

## 📷 Example

```
choose an alias >>> Kavinda
Kavinda has connected to chat room
Kavinda: Hello everyone!
User2: Hi!
```

---

## 🧠 How It Works

* The server listens for incoming TCP connections on port **59000**
* Each client sends an alias during connection
* The server creates a separate thread for each connected client
* Messages received from any client are broadcast to everyone
* If a client disconnects, the server notifies others

---

## 🐞 Error Handling

* Handles unexpected client crashes
* Removes disconnected users cleanly
* Prevents server crashes via exception handling


