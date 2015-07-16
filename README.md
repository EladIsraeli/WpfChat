# WpfChat

### Introduction

A chat application which shares the concept of `Whatsapp`, the application includes a server and client side. The chat system will have a database of users, groups, messages and sessions.

### Required Technologies/Concepts:

* C# .Net 4.5 min
* Wpf (Commands, Behaviors, MVVM, Data-Binding)
* Tcp
* Async/Await
* JSON (optional)
* MongoDB (optional)

### Client Side:

The client application manages the user's groups and message history. 

The client side should use the following technologies:
* Wpf
* .Net 4.5.2

**Features:**

* Connect to the server
* Dashboard with the user's groups
* Each group with it's own page and message history
* Broadcast messages to the group

### Server Side:

The server includes a database of users and groups, and the application that provides the user api.
The database should be implmented using `MongoDB`.

The server application should be implmented using following technologies:
* .Net 4.5.2
* Async/Await programming
* Tcp
* Custom protocol for the communication

**Flow Control**:

On start:

* A user connects to the server 
* The server returns the user's groups
* A dashboad with the user's groups will be rendered to the client

Sending a message: (within a group)

* message is sent to the server 
* the server saves the message in the database 
* broadcast the message to the group's users

### CCP (Custom Communication Protocol)

This is the protocol which the server and the client are using in order to communicate with each other. We will create the protocol.

