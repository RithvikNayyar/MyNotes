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
- **Hypertext**: Text that contains hyperlinks to other documents or resources, enabling non-linear navigation between webpages and forming the interconnected structure of the World Wide Web.
- **Markup Language:** This means that you use "tags" to surround your content, given that content meaning and structure. You are "Marking up" a plain document.
- Together we say that we have created a website in which hyperlink is present. So, I am able to navigate from one page to another.
- To structure our webpage we use HTML Tags. A tag is a label used to define the start and end of an html element. 
	- They are written inside angle brackets: `<tagname>` and `</tagname>`. 
	- Most of the tags comes in pairs like the above one which has both opening and closing tags, but some are self-closing tags Ex: `<br>`.
	- Tags define structure and meaning but not appearance.
	- Tags should be closed using Nesting rule means Tags must be closed in reverse order they were opened.
	  Ex: `<div><p>Hello</p></div>`

**Document Declaration:** 
- Before we even start building the Html page we need to declare the version of the HTML. 
	`<!DOCTYPE html>`
- This declaration is used at very beginning of the document which specify that I am using the latest version of HTML which is version 5. This ensures that webpages is displayed correctly.

- **`<html>`**: The root element that wraps the entire HTML document.

**Head tag:**
- The `<head>` tag is the brain of the HTML document. It contains metadata which is information about the page that helps browsers and search engines understand it.
  
**The Title Tag (`<title>`):** 
- This is the most important element for SEO. It defines the text shown on the browser tab and in google search results.
- **Code:** `<title>My Awesome Portfolio</title>`

**Body element:** The `<body>` tag comes immediately after the closing `</head>` tag and before the final closing `</html>` tag. There is only **one** body element per HTML document.

**Meta Tags (`<meta>`):**
- These are the invisible tags that provide data to the browser and search engines.
- **Charset:** `<meta charset="UTF-8">` (Tells the browser to use standard character encoding so emojis and special symbols display correctly).

- **Heading tags:** Heading tags are used to define titles and subtitles in a webpage. We have six levels of heading tags:
	- `<h1>` : The main Heading/title of the webpage and the highest importance is given to it.
	-  : This covers the major section headings
	- `<h3>` : This covers subsection under the `<h2>` tag.
	- `<h4>`, `<h5>` & `<h6>`: deeper nested subsections and are rarely used.
	  
	- **Not just visual**: While browsers render `<h1>` larger than `<h6>`, the real value is meaning.
	- **Screen readers** use headings to let users navigate pages by jumping between sections (e.g., “Next heading” key).
	- **Search engines** (Google, Bing) use heading structure to understand content relevance and hierarchy — impacting SEO.
>  **Purpose of Headings:** To structure your document in a way that is understandable to both humans and machines. It is not only to make the text big, It is to give the text structural importance.

- **The Paragraph tag `<p>`:** In html the paragraph tag is used to define a paragraph of text. It is one of the most fundamental and frequently used elements for structuring written content on the web.
	- It is a block level element which by default starts on a new line and takes full width by default.
	- Browser automatically add margin before and after each paragraph for visual spacing.
	- Text starts from `<p>` and at the end we have to close by `</p>`. Not a self closing tag.
>  You can think of the paragraph tag as being used to group related sentences and blocks of text into a single, coherent unit.

**Bold, Italic & Underline:** There are many ways to make your text look professional and few of them are:
-  **Bold:** There are 2 tags to make text bold. There are `<b>` which is used to draw attention without adding extra importance and `<strong>` which tells the browser and screen reader that the text has strong importance or urgency.
- **Italic text:** similar to bolding, italics have a same just for looks tag and meaningful tag. 
	- The initial tag `<i>` is used for technical terms, idiomatic phrases, or thoughts. It's for a different voice.
	- The `<em>` emphasis tag is used to stress a specific word. Screen readers will often change the pitch or infection of the voice for this tag.
- **__Underline__:** Underlining is a bit tricky in web design because users often mistake underlined text for clickable link.
	- `<u>` (Underline): Used to represent text that should be rendered with an underline, such as misspelled words.
	```
	<p>This word is <u>mispelled</u>.</p>
	```
> You can nest these tags to apply multiple styles at once.

- **HTML Horizontal rule `<hr>`:** The `<hr>` tag defines a thematic break in a HTML page, and is most often used or displayed as horizontal rule. 
	- While it displays as horizontal rule but it's true purpose is semantic, not visual. It is a self closing tag so no need to close it like paragraph tag.
	- It should not be used merely for decoration or spacing; instead, it conveys structural meaning within the document.
>  You can think of horizontal element is used to separate content on a HTML page.

- **The line break tag `<br>`:** The `<br>` tag in HTML creates a **line break within a block of text**, forcing the content that follows to appear on a new line without starting the new paragraph.
- It is used inline, self-closing tag — no closing `</br>` needed.
>   **Purpose**: Inserts a single line break within a paragraph or inline content.

**Lists in HTML:**
In HTML, lists are used to group related items in a structured and semantic way. There are three main types:
1. **Ordered List `<ol>`:** 
   - Used when the sequence is important.
   - Each item wrapped in `<li>`, which gives default numbering (1,2,3...). We can change this accordingly with letters or roman numbers with type attribute. `<ol type = "A">`
   - Not a self closing tag so when starting we have to use `<ol>` and end with `</ol>`. 
```
<ol type = "A">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```
  
2. **Unordered List `<ul>`:** 
- Used for items without a sequence, or order of the item doesn't matter.
- **Common Use:** Navigation bars, feature lists, or shopping lists.
``` 
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

3. **Description lists `<dl>`:**
- This is a dictionary style list. It consist of pairs of terms and their corresponding description.
- **Tags:** * `<dl>`: The Description List container.
- - `<dt>`: The Description Term (the word).
- `<dd>`: The Description Definition (the explanation).
- **Common Use:** Glossaries, metadata, or FAQ sections.
```
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language.</dd>
  <dt>CSS</dt>
  <dd>Cascading Style Sheets.</dd>
</dl>
```
>  Note: We can put list inside another list. This is how we can create complex multi-level menus like Nested list.

**Comments in HTML:** In HTML, comments are used to leave notes for yourself or other developers within the code. The browser completely ignores them, so they wont show up on the actual webpage.
- `<!--Hello this is a comment in HTML--> ` example of comments.
- In large projects code organization use them to mark start and end of large sections. 
- Sometimes a piece of code breaks and you can comment it out rather than destroying it.
- In collaborations, you are working in teams and you did something complex and want other team members to know why you did this.

**Anchor Tag:**
- The anchor tag is what makes the web "hypertext". It is used to create **hyperlinks**, the very "links" that connects the entire world wide web. Without it, we'd just have isolated documents instead of web.
`The tag = "<a>"`
>  **The purpose:** To make text or an image clickable, allowing users to navigate. 
- It requires an attribute called href(hypertext reference) to specify the destination URL.
  `<a href = "www.google.com">Visit google</a>`
- With anchor tag we can link html pages in our browser.
  `<a href="about.html">Go to About Page</a>`

**Target Attribute:(sub topic anchor tag)**
- The **`target` attribute** in an HTML anchor tag (`<a>`) specifies **where** the linked document or page should open when a user clicks on it.
> The primary reason to use the `target` attribute is to control the **user experience**.

The Four Standard Values
The attribute uses four specific "keywords" that start with an underscore:

1. `_self_`: Opens the link in the same frame as it was clicked (this is the default behavior).
2. `_blank_:` Opens the link in a new window or tab.
3. `_parent_`: Opens the link in the parent frame (used when your page is inside an `<iframe>`).
4. `_top_`: Opens the link in the full body of the window, breaking out of any and all nested frames.















