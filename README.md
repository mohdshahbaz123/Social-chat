# ChatSocial-v1.0

Realtime fully responsive Anonymous Chat App With Users & Rooms - Socket.io, Node & Express

## Screen Shots

![Screenshot 2021-07-17 210244](https://user-images.githubusercontent.com/67598673/126042236-9e53552d-1c0e-42db-97a3-ef885e3cc155.png)
![Screenshot 2021-07-17 210309](https://user-images.githubusercontent.com/67598673/126042240-95e92f1e-863b-4c1f-bb45-89d0e830fe8b.png)
![Screenshot 2021-07-17 210439](https://user-images.githubusercontent.com/67598673/126042237-39d373a7-5aca-46bd-b7c9-56b29c4cb1ee.png)
![Screenshot 2021-07-17 210554](https://user-images.githubusercontent.com/67598673/126042238-017f636e-28ea-4db4-a6ea-8acd9d9fa9e8.png)

### Mobile Responsive

![Screenshot 2021-07-17 210709](https://user-images.githubusercontent.com/67598673/126042239-333342b4-3a6e-4e46-b701-374a98310ec3.png)

## Steps to run 

Like every other node based project just clone it and run `npm install`
this will install all dependencies including dev dependencies.

now to run <br />
`npm run start` <br />
or to run for dev <br />
`npm run dev` (will start nodemon)

### Brief details

Realtime fully responsive Anonymous Chat App With Users & Rooms. <br />
Socket.io is used here for bidirectional and event-based communication from server to client and vice versa.,  <br />
Node as a run-time environment and Express  as a web server on top of which the socketio is sending and receiving request from front to back and so. <br />
momentjs is used for efficient time capture of sending of message in a room.

### Socket programming

Sockets can be thought of as endpoints in a communication channel that is bi-directional and establishes communication between a server and one or more clients. Here, we set up a socket on each end and allow a client to interact with other clients via the server. The socket on the server side associates itself with some hardware port on the server-side. Any client that has a socket associated with the same port can communicate with the server socket. 

### Multi-Threading

A thread is a sub-process that runs a set of commands individually of any other thread. So, every time a user connects to the server, a separate thread is created for that user, and communication from the server to the client takes place along individual threads based on socket objects created for the sake of the identity of each client. We will require two scripts to establish this chat room. One to keep the serving running, and another that every client should run in order to connect to the server. 


### Server Side Script

The server-side script will attempt to establish a socket and bind it to an IP address and port specified by the user (windows users might have to make an exception for the specified port number in their firewall settings, or can rather use a port that is already open). The script will then stay open and receive connection requests and will append respective socket objects to a list to keep track of active connections. Every time a user connects, 
a separate thread will be created for that user. In each thread, the server awaits a message and sends that message to other users currently on the chat. If the server encounters an error while trying to receive a message from a particular thread, it will exit that thread. 





