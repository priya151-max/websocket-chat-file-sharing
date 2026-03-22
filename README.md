# 📡 Media Room Chat and File Sharing Using WebSocket

A real-time communication platform built using **C (Socket Programming)** and the **WebSocket Protocol**, enabling secure private chat rooms and multi-format file sharing.

## 📌 Project Overview

This project implements a real-time chat and file-sharing system using the WebSocket protocol over TCP/IP. It allows users to create private communication rooms and exchange messages and files instantly.

The system demonstrates practical implementation of:

* WebSocket handshake (RFC 6455)
* TCP socket programming
* Frame encoding and decoding
* Masking and unmasking of payloads
* HTTP Upgrade mechanism
* Concurrent client handling using `fork()`

## Demo Video
https://github.com/user-attachments/assets/dd93dab3-a449-458c-ae32-826a03e596c6
## 🏗️ System Architecture

### Architecture Model

* **Client:** C-based WebSocket client
* **Server:** C-based WebSocket server
* **Transport Protocol:** TCP/IP
* **Application Protocol:** WebSocket

### Communication Flow

1. Client establishes TCP connection.
2. HTTP Upgrade request is sent.
3. Server performs WebSocket handshake (SHA-1 + Base64).
4. Persistent full-duplex communication begins.
5. Messages and files are exchanged using WebSocket frames.

## 🚀 Features

* ✅ Real-time bidirectional communication
* ✅ Private room-based chat system
* ✅ Secure WebSocket handshake implementation
* ✅ Multi-format file sharing (PDF, DOCX, PNG, MP3, MP4)
* ✅ Frame masking and unmasking
* ✅ Concurrent client handling using process forking
* ✅ Clean and modular C codebase

## 🧠 Technologies Used

* C Programming Language
* Socket Programming (POSIX)
* OpenSSL (SHA-1 & Base64 Encoding)
* TCP/IP Protocol Suite
* WebSocket Protocol (RFC 6455)

## 📂 Project Structure

```
Media-Room-Chat/
│
├── server.c        # WebSocket Server Implementation
├── client.c        # WebSocket Client Implementation
├── uploads/        # File storage directory
└── README.md
```

## 🔐 Protocols Used

* **HTTP/HTTPS** – For initial handshake and upgrade request
* **WebSocket** – Real-time full-duplex communication
* **TCP/IP** – Reliable data transmission
* **MIME & Multipart** – File handling and format identification

* **HTTP/HTTPS** – For initial handshake and upgrade request
* **WebSocket** – Real-time full-duplex communication
* **TCP/IP** – Reliable data transmission
* **MIME & Multipart** – File handling and format identification

## 📸 Output Demonstration

The system successfully demonstrates:

* Creating private chat rooms
* Joining rooms from different accounts
* Sending and receiving text messages
* Sharing PNG, PDF, DOC, MP3, and MP4 files
* Opening shared files in new tabs or downloading them

## 🎯 Learning Outcomes

Through this project, we achieved:

* Deep understanding of WebSocket protocol internals
* Implementation of SHA-1 hashing and Base64 encoding
* Real-time networking using raw sockets
* Process-based concurrency using `fork()`
* Practical exposure to full-duplex communication systems

## 🔮 Future Enhancements

* User authentication system
* Database integration for persistent chat history
* Cloud storage integration
* AI-powered message summarization
* End-to-end encryption
* Scalable multi-room architecture
