Syllabus:
1. Physical Layer - Cables, Topology, transmission Modes, Encoding, LAN, Devices Modulation
2. Data Link - Stop & Wait, Go Back and selective Repeat, MAC Protocols, Switching, error Control, Ethernet Frame format.
3. Network - IP addressing Routing Protocols, Ipv4 Header, Ipv6 Header
4. Transport - TCP, UDP, Headers
5. Session
6. Presentation
7. Application
8. Network Security

**Computer Network:** It is a collection of various computing devices. The purpose of the computer network is to connect various devices to one another so that they can share the data. In the computer network we have one sender and one receiver. 

Suppose sender is sending some data like a program so how will he share the data?
He needs some sort of connection. Connection can be wired or wireless. Through the connection packets can be sent from one machine to another. 

Now Suppose Sender sends the data and Receiver receives the data, can receiver read or understand the data?
Protocols are running on both ends of devices to make sure that receiver receives the data and reads the data correctly. 

Computer Network is established when a client which is sender and server which is receiver are both different machines.
![[Pasted image 20250120211408.png|472]]

Suppose a machine 1 present in India and machine 2 is present in USA then we need to provide them with some kind of environment so that they can communicate. Computer network is making my process and server's process fell that both are present in the same machine but actually they are not.
**Basic Characteristics of Computer Network**: 
* Fault Tolerance - Ability of computer network to continue to work even after failure and ensure that no loss of data or service.
* Scalability - Ability of the Network to scale itself when load increases and shall maintain performance even under load.
* Quality of Services - the ability to set priorities and manage data traffic to reduce data loss. Delay etc.
* Security - The ability of the network to prevent Unauthorized access, Misuse, Forgery and the ability to provide Confidentiality, Integrity, availability.
There are two types of functionalities one is mandatory and other is option.
Mandatory - when a client sends data some functions are mandatory and cannot be neglected.
1. Error Control - Error control in a computer network ensures that data sent from one device to another arrives accurately and without corruption. It's like a safety net for data.
2. Flow control - Flow control in computer networks is like a traffic cop that ensures data packets travel smoothly between sender and receiver without causing a data jam.
3. Mux and DMUX - Multiplexer combines multiple input into one output signal. Efficiently uses resources like bandwidth. 
* DMUX - Demultiplexer separates one input signal into multiple output signals. Distributes data to different destinations.

Types of Network: 
* PAN - Personal area Network, tech - Bluetooth, IrDA, Zigbee, Range- 1-100 Meter, Transmission speed - Very High, It is private network,  Maintenance is easy and Error rate and cost is low.
* LAN - Local Area Network, Ethernet and Wi-Fi, Up to 2 KM, Speed very high, It is private Network, Maintenance is easy and cost is low.
* WAN - Wide area Network, Leased line is example, Area can be above 50 km, Transmission speed is low, it can be public or private and is difficult to maintain and cost of running is high.
![[Pasted image 20250129111928.webp|639]]

The **physical layer** is the first and lowest layer in the OSI model, responsible for the transmission and reception of raw bit streams over a physical medium. It focuses on hardware, signals, and the physical connection between devices. This layer deals with the **hardware components** and the **physical connection** between devices in a network
###### **Bit Transmission**
- The physical layer is responsible for transmitting raw bits (0s and 1s) over a physical medium (e.g., copper wires, fiber optics, or wireless signals).
- It ensures that the bits are sent and received accurately between devices
###### **Signal Encoding and Modulation**
- Converts digital data (bits) into **signals** suitable for transmission over the physical medium.
- **Encoding**: Maps bits to electrical or optical signals (e.g., Manchester encoding, NRZ).
- **Modulation**: Used in wireless communication to encode data onto carrier waves (e.g., AM, FM, QAM).
###### **Data Rate Control**
- Determines the speed of data transmission (bit rate) based on the medium's bandwidth and quality. Examples: Ethernet standards (10 Mbps, 100 Mbps, 1 Gbps, 10 Gbps). 
###### **Synchronization**
- Ensures that sender and receiver are synchronized so that receiver can correctly interpret the incoming bits and manages timing for bit sampling and transmission.
###### **Physical Topology** 
- Defines the layout of devices and connections in a network.
- Common topologies: 
	- Bus: All devices share a single communication line.
	- Star: Devices connect to central hub or switch
	- Ring: Devices are connected in a circular fashion.
	- Mesh: Devices are interconnected with multiple paths.
###### **Transmission** Mode
- Determines the direction of data flow:
	- Simplex: One way communication
	- Half duplex: two way communication, But not simultaneously
	- Full Duplex: Two way Communication, But Simultaneously
######  **Transmission Media Characteristics**
- Manages the properties of the transmission medium, Such as:
	- Bandwidth - Maximum data transfer rate.
	- Attenuation - Signal loss over distance
	- Latency: Delay in Signal propagation.
	- Noise and Interference: External factors affecting signal quality.
###### **Multiplexing**
- Allows multiple signals to share a single physical medium.
	- Baseband: Uses the entire bandwidth for single signal like ethernet.
	- Broadand: Divides the bandwidth into multiple channels.
######  **Nodes in a Computer Network**
A **node** in a computer network is any **device** or **point** that can send, receive, or process data. Nodes are the fundamental building blocks of a network, enabling communication and resource sharing. Examples of nodes include:
1. **Computers**: Desktops, laptops, servers.
2. **Network Devices**: Routers, switches, hubs, modems.
3. **Peripheral Devices**: Printers, scanners.
4. **IoT Devices**: Smartphones, smart home devices, sensors.
5. **Endpoints**: Any device that communicates over the network.
###### **Roles of Nodes**
1. **Data Transmission**: Send and receive data.
2. **Data Processing**: Perform computations or store data.
3. **Routing**: Forward data to other nodes (e.g., routers).
4. **Resource Sharing**: Provide access to shared resources (e.g., printers, files).
###### **Types of Nodes**
1. **End Nodes**: Devices used by users (e.g., PCs, smartphones).
2. **Intermediary Nodes**: Devices that facilitate communication (e.g., routers, switches).


