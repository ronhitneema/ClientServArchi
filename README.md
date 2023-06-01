# ClientServArchi
The main objective of the project is to develop a secure chat application. We had taken a wide range of literature review in order to achieve all the tasks, where we came to know about some of the products that are existing in the market. We made a detailed research in that path to cover the loop holes that existing systems are facing and to eradicate them in our application. In the process of research we came to know about the latest technologies and different algorithms. As a result, the product has been successfully developed in terms of extendibility, portability, and maintainability and tested in order to meet all the basic requirements.
With the knowledge we have gained by developing this application, we are confident that in the future we can make the application more effectively by adding these services:
•	Extending this application by providing authorisation service.
•	Creating database and maintaining users.
•	Increasing the effectiveness of the application by providing voice chat.
•	Extending it to web support.


The provided code is an example of a simple client-server communication using sockets in C. It creates a TCP connection between a server and a client, allowing them to send and receive messages.

In the server code:

It creates a socket using the socket() function.
Binds the socket to a specific port using the bind() function.
Listens for incoming connections using the listen() function.
Accepts a client connection using the accept() function.
Forks a child process to handle the client connection.
In the child process, it continuously receives data from the client using recvfrom() and sends data back using sendto().
The server code runs indefinitely, accepting new connections and creating child processes for each connection.
In the client code:

It creates a socket using the socket() function.
Sets up the server address and port.
Connects to the server using the connect() function.
Reads user input from the console and sends it to the server using sendto().
Receives the response from the server using recvfrom() and displays it.
Note that the code assumes that the server and client are running on different machines. The client code takes the server's IP address as a command-line argument.

It's important to handle errors properly in a production environment and to perform proper input validation. Additionally, keep in mind that this code does not handle concurrent connections efficiently, as it creates a new child process for each connection. In a real-world scenario, it's advisable to use multithreading or other methods to handle concurrent connections more effectively.
