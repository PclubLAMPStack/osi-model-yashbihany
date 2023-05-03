# The OSI Model -

The OSI(Open systems interconnection) model describes data communication between different computer systems.It consists of seven layers, each responsible for a specific aspect of network communication:

***
**1) Physical layer** :

The physical layer is responsible for transmitting data over a physical medium. Examples of physical layer technologies include Ethernet, Wi-Fi, Bluetooth, and USB.

The physical layer defines the physical characteristics of the transmission medium, such as voltage levels, signal timing, and physical connectors. It also defines the types of signals used to represent digital data, such as amplitude modulation, frequency modulation, or phase modulation.
***
**2) Data Link Layer** :

The Data Link Layer is the second layer of the OSI model and is responsible for providing reliable data transfer across the physical layer by adding framing, error detection, and correction. The Data Link Layer also controls access to the physical medium, resolves collisions, and performs flow control to ensure that data is transmitted at an appropriate rate.

The Data Link Layer uses several protocols to perform its functions.For example, Ethernet is a widely used LAN protocol that provides reliable data transfer between devices on the same physical network. Other data link layer protocols include Point-to-Point Protocol (PPP), High-Level Data Link Control (HDLC), and Asynchronous Transfer Mode (ATM).

Error detection and correction are achieved by adding a frame check sequence (FCS) to the data that is transmitted.
Flow control is achieved by using techniques such as buffering and <u> *windowing** </u> to ensure that data is transmitted at an appropriate rate. 
***
**3) Network Layer** :

This layer is responsible for routing data across multiple networks, using logical addresses(IP addresses) to determine the best path for data to travel. Examples of network layer protocols include the Internet Protocol(IP), the Routing Information Protocol (RIP), and the ICMP.

Terminologies: 

- *Internet Protocol (IP)* : This is the primary protocol used by the network layer to route data between different networks. IP addresses are used to identify individual devices and to direct data to the correct destination.

- *Internet Control Message Protocol (ICMP)* : This protocol is used for error reporting and diagnostics in IP networks. For example, if a packet is lost or cannot be delivered, ICMP messages can be used to alert the sender or recipient of the problem.

- *Routing*: The network layer is responsible for routing data between different networks, using routing algorithms and protocols to determine the best path for data to travel. Routing protocols include OSPF, <u>*BGP**</u>, and <u>*RIP**</u>, among others.
***
**4) Transport Layer**: 

It provides reliable end-to-end communication between applications running on different devices. It is responsible for managing data flow control, segmentation, and reassembly.The transport layer is critical for ensuring that data is transmitted accurately and reliably between devices.

The two main transport layer protocols :

- *Transmission Control Protocol (TCP)* :

TCP provides reliable, ordered, and error-checked delivery of data between applications. It establishes a connection between two endpoints, manages data transfer, and ensures the data is delivered in the correct order. TCP is used for applications that require reliable data transmission, such as web browsing, file transfers, and email.

- *User Datagram Protocol (UDP)* :

UDP is a connectionless protocol that provides unreliable, unordered, and unchecked data delivery between applications. It is used for faster, less reliable data transmission applications, such as real-time video or audio streaming, online gaming, and <u>*VoIP**</u>.

The transport layer also provides port numbers, identifying specific applications running on a device. The source and destination port numbers are combined with the IP address to identify the specific application sending or receiving data. For example, web traffic typically uses port 80 or 443, while email traffic uses port 25 or 587.
***
**5) Session Layer**: 

It establishes, manages, and terminates communication sessions between applications. These sessions provide a way for applications to exchange data with each other in a structured and secure way.

Several session layer protocols are commonly used. For example, the Remote Procedure Call (RPC) protocol, is used to enable a client application to call a function or method on a remote server application and receive the results back. Another example is the Secure Sockets Layer (SSL) or Transport Layer Security (TLS) protocol, which provides secure communication between a client and server by encrypting the data being exchanged.

The session layer also provides session recovery services, which allow a session to be reestablished in the event of a communication failure.
***
**6) Presentation Layer** :

The Presentation Layer uses protocols and services to transform data from one representation to another. Some of the protocols used at the Presentation Layer include:

- ASCII(American Standard Code for Information Interchange) is a character encoding standard used to represent text in computers.

- EBCDIC(Extended Binary Coded Decimal Interchange Code) is a character encoding used mainly on IBM mainframe systems.

Unicode: Unicode is a character encoding standard that supports a wide range of characters from different languages and scripts.

MIME(Multipurpose Internet Mail Extensions) is a protocol used for sending email messages with attachments.

It also provides services such as data compression(like JPEG and MPEG which reduce the size of multimedia files) and data translation(for example the data translation service ensures that a  file created on a Mac system should be in the same format as the same file created on a Windows computer)

**7) Application Layer** :

It iss where application-specific protocols are implemented to enable users to access various network services such as email, web browsing, file transfer, and remote login. The application layer interacts with the lower layers of the OSI model to establish communication sessions and transmit data between applications.

The application layer includes a number of protocols that allow different applications to communicate with each other over the network. Some examples of application layer protocols include HTTP (used for web browsing), SMTP (used for email), FTP (used for file transfer), Telnet (used for remote login), and DNS (used for domain name resolution).

Thus, it provides a variety of services to end-users, such as email, file transfer, remote access, and web browsing. These services are typically provided through application software that runs on a user's computer, such as a web browser, email client, or file transfer client.

For example, when a user wants to browse a website, their web browser application will use the HTTP protocol to request data from the server, which is then transmitted over the lower layers of the OSI model (transport, network, data link, and physical layers) to reach the destination server.

---

# Example of how it works!

Here are the steps to create a server using the OSI model:

- **Physical Layer:** The first step is to set up the physical layer, which involves choosing the hardware and physical medium that will be used to transmit data. This could include selecting a server computer, network adapters, Ethernet cables, and switches.

- **Data Link Layer:** Once the physical layer is set up, the data link layer needs to be configured to provide error detection and correction and to ensure that data is transmitted reliably. This could involve setting up the Ethernet protocol, which operates at the data link layer, to enable communication between devices.

- **Network Layer:** The next step is to set up the network layer, which is responsible for routing data between devices. This could involve configuring the IP protocol to assign IP addresses to the server and other devices on the network, and setting up routing tables to ensure that data is transmitted to the correct destination.

- **Transport Layer:** The transport layer is responsible for ensuring that data is transmitted reliably and that communication sessions are established between applications. To set up a server, you would need to configure a transport layer protocol, such as TCP or UDP, to enable communication between the server and client applications.

- **Session Layer:** The session layer is responsible for managing communication sessions between applications. To set up a server, you would need to implement session management protocols, such as Remote Procedure Call (RPC), which enables a client application to call a function on the server application.

- **Presentation Layer:** The presentation layer is responsible for data representation and encryption. To set up a server, you may need to implement data encryption protocols, such as Secure Sockets Layer (SSL) or Transport Layer Security (TLS), to ensure that data is transmitted securely over the network.

- **Application Layer:** Finally, the application layer is where server-specific protocols and services are implemented. To set up a server, you would need to choose and implement the appropriate application layer protocols for the services you want to provide, such as HTTP for web servers, SMTP for email servers, or FTP for file servers.

---

**Windowing* : Windowing specifies a window size, which is the maximum amount of data the sender can transmit at any given time.The receiver can also specify a window size, which tells the sender the maximum amount of data that the receiver can receive at any given time. This helps to prevent data loss due to congestion and ensures that the data is transmitted reliably and efficiently.

**BGP*(*Border Gatewar Protocol*) : BGP is an exterior gateway protocol, which means it is used to route traffic between different organizations rather than within a single network. BGP is responsible for exchanging information about network reachability and the paths traffic should take to reach its destination. It uses a variety of attributes, such as the Autonomous System Path (AS_PATH), to determine the best path for traffic based on network policies.

**RIP*(*Routing Internet Protocol*): RIP works by having each router broadcast its routing table to its neighboring routers, which broadcast their own routing tables to their neighbors. Each router then combines the routing information it receives from its neighbors with its own routing table to determine the best traffic path.

**VoIP*(*Voice over Internet Protocol*): It is a technology that allows voice communication to be transmitted over the Internet using IP networks, rather than traditional phone lines. VoIP converts analog audio signals into digital data packets, which are transmitted over IP networks, then converted back to analog audio signals at the receiving end.

---

<h1 align="center">Thank You!!</h1>
