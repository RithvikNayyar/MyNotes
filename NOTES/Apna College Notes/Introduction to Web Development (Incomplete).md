#### Basics:
**What is the Internet?** 
- The **Internet** is like a **huge worldwide network** that connects millions of computers, phones, and devices so they can share information with each other.
- In order to send or receive data, computers are given special IP address to communicate with each other. EX:- 192.168.0.1
![[image-1.png]]

**What are IP addresses?** 
- **IP address** (Internet Protocol address) is a numerical label assigned to every device connected to a computer network that uses the Internet Protocol for communication.
- **Purpose**: Identifies and locates devices on a network (like a postal address for data delivery).
**Two Main Types**:
- **IPv4**: 32 bit binary number format typically represented in dotted-decimal notations, divided into 4 octets (8 bit each) range: `0.0.0.0` to `225.225.225.225`.
	- Has slower routing and less efficient, still dominating but now fading away slowly.
  > In 2011 we have already exhausted all the IPv4 addresses and now ISP reuses the exhausted IP address via NAT, IPv6 transition, and address trading.

- **IPv6:** 128 bit binary number, represented in hexadecimal, separated by colons: `2001:0db8:85a3::8a2e:0370:7334`.
	- Every device gets individual IP address.
	- Has faster routing, better security (IP-sec Built-in).

**What is DNS?** 
- Domain Name system - It translate human readable domain name like `google.com` into IP address like 8.8.8.8.
- So the browser can now load the website. It is like phone-book where the name and address of the website is stored.
**Working of DNS:**
1. **User enters a URL** (e.g., `www.example.com`) into the browser.
2. **The browser checks its local cache** to see if it already has the corresponding IP address. If found, it skips further steps.
3. If not found, the **operating system** queries a **recursive DNS resolver** (usually provided by the ISP or a public DNS like Google or Cloudflare).
4. If the resolver doesn’t have the record cached, it begins a **recursive lookup**:
    - First, it queries a **root nameserver**.
        > There are 13 logical root server clusters worldwide (though each runs many physical servers for redundancy).
    - The root server responds with the address of the appropriate **Top-Level Domain (TLD) server** (e.g., `.com`, `.org`, `.in`).
5. The resolver then queries the **TLD server** for the domain’s authoritative nameserver.
    - For `www.example.com`, it asks the `.com` TLD server: _“Who is responsible for example.com?”_
6. The TLD server returns the address of the **authoritative nameserver** for that domain.
7. The resolver queries the **authoritative nameserver** — the server that holds the actual DNS records for the domain.
8. The authoritative nameserver returns the **IP address** for `www.example.com`.
9. The resolver caches the result and sends the IP back to the browser.
10. The browser uses the IP address to establish a connection and load the website.
- For more information on the dns records or IP address we can look up in `nslookup.io`. 

**Mac Address:** A mac address (Media access control address) is a unique 12-digit hardware identifier assigned to every network-enabled device like laptop, mobiles or router. It's Hard-coded into the device's network interface card (NIC) by the manufacturer.
- Format : `00:1A:2B:3C:4D:5E` 
- Used at the data link layer (layer 2) of the network to identify the devices on the same local network.
- Unlike IP addresses (which can change), MAC addresses are permanent (unless manually spoofed).
- **WORKING:** When device send data, It checks client's mac address as source and target's mac address as destination.
>  IP address are dynamic and goes away once source machine are turned off, But Mac addresses are permanent.
>  The problem with only IP addresses are that if by any chance i disconnect from the network while sending the request, The person who gets the same IP will also get my requested data.

**What are Port Numbers?** 
- Port Numbers are a number range - `0 - 65535` that identifies a specific service/app on a device. Ex: Instagram, whatsapp.
- Your device has one IP address but many port numbers so that it can identify which app/service on your device has requested that data.
  So, IP = Apartment address, & Port = Apartment Number
- From port `0 - 1023` are reserved for system services and some well known ports are:
	- `80` - HTTP
	- `443` - HTTPS
	- `22` - SSH
	- `3306` - MySQL
- From port `1024 - 48151` are used by apps.
- From port `49152 - 65535` are Temporary ports used by clients in browser.

**What is HTTP Network?**
- **HTTP** is Hypertext transfer protocol
- It's a protocol used to transfer web pages (HTML, images, etc.) between a client and the server over the internet.
- It is Not Encrypted, No authentication. and Insecure so avoid login and payments.
- Data is sent as plain text so it is easy to steal by hackers.
- Port Number is `80`.
- Mostly used for Static websites.

**What is HTTPS Network?**
- **HTTPS:** Hypertext transfer protocol secure (SSL/TLS encryption). It's Secure version of HTTP.
- Encrypts data between browser and server with TLS/SSL encryption. Basically, server is authenticated via certificate.
- Data is Encrypted so it prevents eavesdropping, tampering and impersonating. Basically, safe from stealing.
- Port Number is `443`.  It's secure so all login apps use it
- It is mandatory for all modern websites.

**What is LAN (Local area Network)?**
- It is a computer network that interconnects devices within a limited area such as home, school, office.
- Speed can range from `1Mbps to 10+ Gbps`, area can be within 1 KM.

**What is WAN (Wide area Network)?**
- A wide area network connects multiple LAN's across large geographical distances and often using public infrastructure or leased lines.
- Mostly used by ISP like Airtel, JIO, AT&T etc, where it can reach whole city, country or global.
- Speed depends on the link like fiber, satellite and latency is higher as distance is huge.
- Ownership is often shared between ISP, private Owners & government.

**What is a Switch?** 
- A Network switch is a device that connects multiple devices in a LAN and forwards data only to the intended recipient.
- It uses Mac address and ports to identify the request.

**What is a Router?**
- A router is a device that connects different networks and forwards packets based on IP addresses.
- It routes data packets from the network. Like home>server.
**Additional Functions:**
- Firewall (blocks unsolicited inbound traffic).
- DHCP server (assigns private IP's in LAN).
- DNS resolver (caches/forwards DNS queries).
- Wireless access point (in home “wireless routers”).

**What are Private IP Addresses?**
- IP addresses reserved for use **only inside private networks** (LANs). Not routable on the public internet.
- Uses: Solve IPv4 address shortage via NAT.
- Enhances security and simplifies network Management.
- Limitation: Cannot be used directly to the internet - Must be translated (via NAT) to a public IP.

**What are Public IP Addresses?**
- Globally unique IP addresses assigned by ISP's .
- Assigned to you via router One public IP for entire household. And general users get dynamic IP. 
- Static IP's are provided to servers, cloud VM's, email servers, basically which runs 24/7

**What is Web Development?** 
- Building websites for the Internet. 
- It usually includes:
	- Front-end — what users see (design, buttons, pages)
	- Back-end — how things work behind the scenes (servers, databases, logic)
- Example - For `amazon.in` request is made to amazon server and in response we get the front-end shown in the browser consisting of HTML, CSS, JS. 
- This is known as **Request-Response cycle**.

- **HTML**: It is used to build **structure** of the website. 
- **CSS**: This styles the page, adding visual appeal by controlling layout, fonts, colors, and even animations.
- **JS**: Adding **functionality** on it like the buttons and all we have created making those work. we can make animation using java script. 
- When these three technologies are combined then it is called front-end technologies.

#### HTML 
- Hypertext markup language - this tells us about what is the structure and formatting of the website.
- The backbone of the webpage, it structures the content and provides the semantic meaning (like headings, paragraphs, images, links, etc.).