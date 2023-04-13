# Python Chat Client and Server

This repository contains two Python programs for a text-based chat application:

1. Chat Client (client.py)
2. Chat Server (server.py)

These programs use Python, sockets, and the Transmission Control Protocol (TCP) to create a simple chat application that allows users to exchange messages with each other.

## Chat Client (client.py)

The chat client allows users to connect to the chat server and exchange messages with other users. It provides a user-friendly text-based interface for chatting.

### Features

1. Connects to the chat server and lets the user log in using a unique name.
2. Asks for another name if the chosen name is already taken.
3. Lets the user shutdown the client by typing !quit.
4. Lets the user list all currently logged-in users by typing !who.
5. Lets the user send messages to other users by typing @username message.
6. Receives messages from other users and displays them to the user.

### Usage

To run the chat client, execute the following command:

```bash
python3 client.py <server_address> <server_port>
```

Replace <server_address> and <server_port> with the appropriate values for your chat server.

Chat Server (server.py)
The chat server connects multiple clients and forwards messages between them using the same chat protocol as the client.

Features
Supports the full protocol specified in Appendix A.
Supports at least 64 simultaneous clients.
Usage
To run the chat server, execute the following command:
```bash
python3 server.py <server_port>
```
Replace <server_port> with the desired port for your chat server.

