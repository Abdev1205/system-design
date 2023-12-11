# TCP/IP Model

The **Transmission Control Protocol/Internet Protocol (TCP/IP)** is a practical network model developed by the Department of Defense (DoD) in the 1960s to facilitate communication between diverse network devices on the internet.

## Layers of TCP/IP Model

### Physical Layer 💻

The **Physical Layer** translates message bits into signals for transmission on a medium. It is where real communication takes place. Characteristics include topology (bus, star, hybrid, mesh, ring), line configuration (point-to-point, multipoint), and transmission mode (simplex, half-duplex, full-duplex).

### Data Link Layer (DLL) 📡

The **Data Link Layer** is subdivided into two layers: **MAC (Media Access Control)** and **LLC (Logical Link Control)**. MAC is responsible for data encapsulation (framing) of IP packets into frames, while LLC deals with flow control and error control.

### Network Layer 🌐

The **Network Layer** adds IP addresses (logical addresses) to data segments to form IP packets and determines the best path for data delivery. Protocols include:

- **IP (Internet Protocol)**: Determines the best path for packet delivery using IP addresses.
- **ARP (Address Resolution Protocol)**: Finds MAC/physical addresses from IP addresses.
- **ICMP (Internet Control Message Protocol)**: Responsible for error reporting.

### Transport Layer 🚢

The **Transport Layer** manages flow control, end-to-end connectivity, and error-free data transmission. Protocols are:

- **TCP (Transmission Control Protocol)**: Connection-oriented, reliable protocol that segments, assigns sequence numbers, and ensures error correction and proper data delivery order.
- **UDP (User Datagram Protocol)**: Connectionless, less reliable, and cost-efficient protocol without segmentation and error checking.

### Application Layer 📱

The uppermost layer combines the OSI model's session, presentation, and application layers. Users interact with applications and access network resources through this layer. Protocols include:

- **HTTP (Hypertext Transfer Protocol)**: Used to access data on the World Wide Web.
- **DNS (Domain Name System)**: Translates domain names to IP addresses.
- **SMTP (Simple Mail Transfer Protocol)**: Used to send Email messages.
- **FTP (File Transfer Protocol)**: Used to transfer files between computers.
- **TELNET (Telecommunication Network)**: A two-way communication protocol connecting a local machine to a remote machine.

## OSI Vs TCP/IP
 ![](https://i.postimg.cc/CKJCw2Zh/image.png)

## How TCP/IP Model works in real life

![](https://i.postimg.cc/qqVwD5zp/image.png)
