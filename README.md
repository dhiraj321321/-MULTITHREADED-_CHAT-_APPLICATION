# -MULTITHREADED-_CHAT-_APPLICATION
**COMPANY**: CODTECH IT SOLUTIONS

**NAME**: DHIRAJ PARIDA

**INTERN ID**:CT08EMF

**DOMAIN**:JAVA DEVELOPMENT

**BATCH DURATION**: January 5th, 2025 to February 5th, 2025

**MENTOR NAME**: Neela Santhosh Kumar 

**DESCRIPTION OF TASK**:The Client-Server Chat Application is a very simple real-time chat system through which multiple clients can communicate with each other with a central server. It uses Java Sockets for communication through a network and multithreading for dealing with multiple client connections. In such a way, all clients can send messages and concurrently receive them without blocking each other.

Technologies Used: Java Sockets is applied in this application to handle the network communications between the server and its respective clients.
Multithreading: To handle multiple clients at a time by creating a new thread for each client connection.
Java I/O: For reading from and writing to the network streams for communication.
Compiler and IDE Used:
Compiler: The project was compiled using the Java Development Kit (JDK). The specific version of JDK used for this project is JDK 8 or above (recommended version for compatibility).
IDE: The project is developed in Apache NetBeans or any other IDE that supports Java development such as Eclipse or IntelliJ IDEA.
NetBeans: NetBeans is used to create, compile, and run the project. It provides integrated support for Java Sockets and Multithreading, making it ideal for developing this type of network-based application.
Components:
ChatServer.java (Server Side):
The server listens for incoming connections from clients on a specific port.
When a client connects, the server creates a new thread (ClientHandler) to handle communication with that client.
The server keeps track of all connected clients and broadcasts any received messages to all clients, ensuring that all clients are updated in real-time.
The server logs every broadcast message for debugging and monitoring purposes.
ChatClient.java (Client Side):

The client connects to the server and listens for messages from other clients.
The client will enable the user to type and send messages to the server. Once a message is sent, it will be broadcasted to all other connected clients.
Each client will listen for incoming messages from the server and display them in real-time.
Key Features:
Real-time Communication: Clients can send and receive messages in real-time.
Multithreading: Each client runs in its own thread, ensuring that multiple clients can interact with the server concurrently without blocking.
Broadcasting: If one client sends a message, the server broadcasts to all other connected clients.
Server Logging: The server logs all the messages it receives and broadcasts for monitoring communication.
How It Works:
Server Initialization:

The server is started by running ChatServer.java, which listens for incoming connections on port 12345. Once a client connects, the server creates a new ClientHandler thread to handle communication with that client.

A different client is run for each one by running the ChatClient.java. The client connects to the server using its IP address and port.
Messages can then be sent from the client to the server, and the server can broadcast them to all connected clients.
Message Broadcasting:

When a message is sent from a client, the server captures it and makes a call to the broadcast method, which propagates the message to all clients connected.
Every client captures the message and presents it to the user.
Multithreading:

The server uses threads to handle every client connection. Therefore, the server can communicate with several clients concurrently without blocking.
The ClientHandler class is the one that manages the input and output streams of every client.
Project Flow:
Start the Server:
Run ChatServer.java
The server is waiting for connections from clients at port 12345.
Start Several Clients:
Run several instances of ChatClient.java on different computers or in various console windows.
Clients connect to the server and can send and receive messages.
Message Exchange:

After a client sends a message, it is broadcasted to all other connected clients, who can then respond in kind.
Termination:

The server and clients can be terminated by closing the console or stopping the execution of the Java programs.
Where This Project Can Be Applied:
Internal Messaging Systems for Organizations:

This messaging application can be used as the internal messaging system of organizations, where employees can communicate in real-time. It can be extended to include authentication, channels, and more.
Small-Scale Multiplayer Games:

The client-server architecture can be used to facilitate real-time communication between players in small-scale multiplayer games. Players can exchange messages, chat during the game, or even form teams.
Customer Support Systems:

The application can be extended to be used as a live chat system for customer support systems where agents and customers can chat with each other.
Learning Platforms:

The project can be used in e-learning platforms for real-time communication between instructors and students during online classes or discussions.
Collaborative Tools:

The project can be used as a foundation for collaborative tools where team members can discuss and share ideas in real time, especially in environments where quick communication is required.
Prototyping Network Communication:

The chat application is a basic prototype to demonstrate network communication using Java Sockets, making it ideal for educational purposes in teaching network programming and multithreading.
Expected Output:
Server Console:

The server prints logs of all incoming messages and broadcasts.
Example log: Broad-casting message: Hello, Client 1!
Client Console:

Any client can instantly see messages sent out by other clients.
Example output from a client: Hello, Client 1!
Conclusion
This project shows a practical hands-on way that client-server communi-cations and multithreaded program-ming concepts can be explored. The application would be extended on to add functionality such as the ability to share files, introduce private messaging features, or bring in user authorization.

**OUTPUT**:
![Image](https://github.com/user-attachments/assets/00c3d448-e815-47b6-ad21-d394ecec9e14)
![Image](https://github.com/user-attachments/assets/4569e596-27a6-4b89-b2c0-5b8a4d473298)
![Image](https://github.com/user-attachments/assets/6bd7126a-8960-475f-871d-ad287fa34922)
