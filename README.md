# Client-Server-File-Transfer-System
The primary objective was to create a client-server environment capable of copying the contents of a file from the client to the server. This system was designed to mimic a file UPLOAD process, where the client code runs as a single process, and the server code runs as a separate process on the same computer.

In this project, I developed a robust Client-Server File Transfer System for Trent University's COIS3380H course. The system is designed to facilitate efficient and reliable file uploads from a client to a server, mimicking a real-world file upload process. 

**Technologies Used:**

**Language: C**
Communication Channels: IPC using FIFO, Shared Memory, and Sockets and Client-Server
Tools: read() and write() system calls, TCP/IP sockets, shared memory segments
Project Details:

**Communication Channel Options:**

IPC using FIFO: Implemented two FIFOs for client-to-server and server-to-client transfers.
Shared Memory: Utilized a shared memory segment for a more complex, synchronized communication.
Sockets and Client-Server: Established a real client-server environment using TCP/IP sockets.
Functionality:

The system allows the filename to be supplied to the client as a command-line parameter.
The client sends a message containing the filename to the server.
The server prepares to receive data and the client begins the file transfer through the chosen communication channel.
Data packets are structured to include both the number of bytes being transferred and the data stream.
The server writes the received data to a local file, handling arbitrary file lengths and different block sizes.
Restrictions and Special Considerations:

Used open() and read() for data retrieval to ensure binary file compatibility.
Avoided bulk transfer utilities to demonstrate fundamental data transfer techniques.
Implemented proper closing of files and graceful disconnection after the transfer.
Testing and Validation:

Conducted extensive testing with files of various sizes and types, including non-text files.
Validated file integrity post-transfer using the md5sum program to compare source and target files.

**Conclusion:**
This Client-Server File Transfer System project not only demonstrates my ability to adhere to strict specifications and deadlines but also showcases my skills in creating efficient and reliable software solutions. The project was a valuable opportunity to deepen my understanding of client-server architecture, communication protocols, and system-level programming in C.


