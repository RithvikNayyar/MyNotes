#### Basics:
**What is the Internet?** 
- The **Internet** is like a **huge worldwide network** that connects millions of computers, phones, and devices so they can share information with each other.
- In order to send or receive data, computers are given special IP address to communicate with each other. EX:- 192.168.0.1
![[image-1.png]]

**What is DNS?** 
- Domain Name system - It translate human readable domain name like `google.com` into IP address like 8.8.8.8.
- So the browser can now load the website. It is like phone-book where the name and address of the website is stored.
**Working of DNS:**
1. **User enters a URL** (e.g., `www.example.com`) into the browser.
2. **The browser checks its local cache** to see if it already has the corresponding IP address. If found, it skips further steps.
3. If not found, the **operating system** queries a **recursive DNS resolver** (usually provided by the ISP or a public DNS like Google or Cloudflare).
4. If the resolver doesn’t have the record cached, it begins a **recursive lookup**:
    - First, it queries a **root nameserver**.
        > 🌐 There are 13 logical root server clusters worldwide (though each runs many physical servers for redundancy).
    - The root server responds with the address of the appropriate **Top-Level Domain (TLD) server** (e.g., `.com`, `.org`, `.in`).
5. The resolver then queries the **TLD server** for the domain’s authoritative nameserver.
    - For `www.example.com`, it asks the `.com` TLD server: _“Who is responsible for example.com?”_
6. The TLD server returns the address of the **authoritative nameserver** for that domain.
7. The resolver queries the **authoritative nameserver** — the server that holds the actual DNS records for the domain.
8. The authoritative nameserver returns the **IP address** for `www.example.com`.
9. The resolver caches the result and sends the IP back to the browser.
10. The browser uses the IP address to establish a connection and load the website.
- For more information on the dns records or IP address we can look up in `nslookup.io`. 


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