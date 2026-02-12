#### Basics:
**What is the Internet?** 
- The **Internet** is like a **huge worldwide network** that connects millions of computers, phones, and devices so they can share information with each other.
- In order to send or receive data, computers are given special IP address to communicate with each other. EX:- 192.168.0.1
![[image-1.png]]

- Suppose I am the client and I have sent request for google.com then my request goes to the following:
1. ISP - ISP checks in the cache data weather the IP address for google.com is available or not.
2. DNS - If not available then it sends request in DNS(Domain Name system), It is like the phone book which holds all the website details.
3. Client - Then the DNS sends back the IP address to ISP and likewise ISP shares the IP address to Client, and now Client is able to open that website.
- For more information on the dns records or IP address we can look up in `nslookup.io`. 

**What is Web Development?** 
- Building websites for the Internet. 
- It usually includes:
	- Front-end — what users see (design, buttons, pages)
	- Back-end — how things work behind the scenes (servers, databases, logic)
- Example - For `amazon.in` request is made to amazon server and in response we get the front-end shown in the browser consisting of HTML, CSS, JS. 
- This is known as **Request-Response cycle**.

- **HTML**: It is used to build **structure** of the website. 
- **CSS**: It is used to **style** the things on the structure we have build. Ex: Color, font, etc.
- **JS**: Adding **functionality** on it like the buttons and all we have created making those work. we can make animation using java script. 
- When these three technologies are combined then it is called front-end technologies.

#### HTML 
- Hypertext markup language - this tells us about what is the structure and formatting of the website.
- The backbone of the webpage, it structures the content and provides the semantic meaning (like headings, paragraphs, images, links, etc.).