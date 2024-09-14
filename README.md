# How the Internet Works When You Search for a URL

1. **DNS Lookup**:  
   When you enter a URL, your browser contacts a Domain Name System (DNS) server to convert the human-readable URL (like `example.com`) into an IP address, which identifies the server hosting the website.

2. **Signal Transmission**:  
   Your request is transmitted from your device (laptop, phone, etc.) to your router. The router sends the data to your Internet Service Provider (ISP). If you're using Wi-Fi, your data is sent as radio waves to your router, which then sends it to your ISP's network.

3. **ISP Routing**:  
   The ISP routes your request over its network. It checks if the requested website is accessible (i.e., not blocked or blacklisted), and then forwards the request through multiple network nodes (like hubs, routers, and data centers) until it reaches the destination server.

4. **Server Response**:  
   Once your request reaches the server hosting the website, the server processes it and sends the requested webpage data back. This return data follows the same path back to your device through the ISP’s network.

5. **Rendering**:  
   Your browser takes the data from the server (usually in the form of HTML, CSS, JavaScript, etc.) and displays the webpage you requested.

---

**Note**:  
The transmission from your device to the nearest hub or tower is often a combination of radio waves (for wireless communication) and electrical signals (for wired connections). However, the routing and data delivery between servers and networks mainly happen over high-speed fiber optic cables, which use light pulses to transmit data rapidly over long distances.

---

# What is an IP Address?

An **IP address** is like the address of your device on the internet. It’s assigned by your **Internet Service Provider (ISP)** whenever your device connects to the internet. This allows your device to communicate with websites, services, and other devices. The assignment of IP address is based on a protocol called DHCP (Dynamic Host Configuration Protocol). 

There are two main types of IP addresses:

1. **IPv4 (Internet Protocol Version 4)**:
   - This is the older version and looks something like this: `192.168.1.1`.
   - It uses 32-bit numbers, which means there are about 4.3 billion unique addresses available.
   - However, because so many devices are connected to the internet today, we started running out of IPv4 addresses.

2. **IPv6 (Internet Protocol Version 6)**:
   - This is the newer version and looks like this: `2001:0db8:85a3:0000:0000:8a2e:0370:7334`.
   - It uses 128-bit numbers, which provides **trillions** of unique addresses, solving the shortage problem.
   - This is why IPv6 was created—to ensure there are enough addresses for all the devices connecting to the internet now and in the future.

---

## Difference Between Public and Private IPs

- **Public IP Address**:  
  A public IP is the address that is assigned to your device by your ISP and is visible on the internet. When you visit a website, your public IP is used to communicate with servers across the web.

- **Private IP Address**:  
  A private IP is assigned to devices within your local network (like your home Wi-Fi). For example, your computer, phone, and smart devices might have private IP addresses like `192.168.0.5` or `10.0.0.2`. These addresses are not visible to the outside world and are used only for communication within your home network.


Think of your **private IP** like a **nickname** that your family or close friends use at home—it's only used within your private circle. 

On the other hand, your **public IP** is like your **formal name (Ashutosh Panda)** that is used outside, like at school or in public spaces, to identify you to the world.

---

In simple terms, **public IP** is used to communicate with the world, and **private IP** is used to communicate with devices in your home or office network.

---

# What is a MAC Address?

A **MAC (Media Access Control) address** is a unique identifier given to a device's network card, allowing it to communicate on a local network like Wi-Fi or Ethernet. It is a hardware address that is hardcoded into your device's network card by the manufacturer.

### Key Points:

1. **Format**:
   - A MAC address is a 12-character code, often separated by colons or hyphens.
   - Example: `00:1A:2B:3C:4D:5E` or `00-1A-2B-3C-4D-5E`.

2. **Purpose**:
   - It is used to identify devices on a local network.
   - Works on the **Data Link Layer (Layer 2)** of the OSI model.

3. **Uniqueness**:
   - Every MAC address is supposed to be unique to each device.

4. **Types of MAC Addresses**:
   - **Unicast MAC**: For a single device.
   - **Multicast MAC**: For multiple devices.
   - **Broadcast MAC**: For all devices in the network.

5. **Static Nature**:
   - Unlike an IP address, a MAC address is usually **permanent** and does not change.

6. **Difference Between MAC and IP Address**:
   - **MAC Address**: Identifies a device on a local network.
   - **IP Address**: Identifies a device across the internet.

7. **Security**:
   - MAC addresses can be **spoofed** (faked) to pretend to be another device.

8. **Uses**:
   - MAC addresses are used in **Ethernet, Wi-Fi, and Bluetooth** to manage how devices talk to each other.

---

### Example Interview Question:

**Q**: *What's the difference between a MAC address and an IP address?*  
**A**: A MAC address is a hardware identifier unique to a device, used on local networks. An IP address is assigned to the device to identify it across the internet.

---
# What is a Proxy in Computer Networking?

A **proxy** in computer networking is a server that acts as an intermediary between a user's device and the internet. When you use a proxy server, your internet traffic is routed through it before reaching the website or service you're trying to access. This can help with functions like security, privacy, or bypassing restrictions.

### How Does a Proxy Work?

1. You send a request (like accessing a website) to the proxy server.
2. The proxy forwards the request to the destination website.
3. The website responds to the proxy, which then sends the response back to you.

In this way, the proxy acts as a middleman, hiding your IP address and making it seem like the request came from the proxy instead of your actual device.

### Uses of a Proxy:

1. **Privacy**: It hides your IP address, providing some level of anonymity online.
2. **Security**: Can filter and block malicious content.
3. **Access Control**: Restricts access to certain websites or content.
4. **Bypassing Restrictions**: Can be used to bypass geo-restrictions or local network restrictions.

---

### Example Scenario (University Network):

In a university, students might be restricted from accessing specific websites, like social media or streaming platforms. To enforce this, the university can set up a **proxy server**. When a student tries to access a blocked site, the proxy checks the requested website against a list of restricted sites. If it’s on the list, the proxy denies access, showing a message like "Access Denied."

Conversely, some students might try to bypass the university’s restrictions by setting up their own **proxy** or using a public one. By doing this, their traffic would be routed through that external proxy, making it appear like they’re accessing the site from outside the university network, allowing them to access restricted content.

---

### Interview-Friendly Explanation:

**Q**: _What is a proxy in computer networking, and how is it used?_  
**A**: A proxy is a server that sits between a user’s device and the internet. It forwards requests to websites and services on behalf of the user, often hiding their IP address. Proxies can be used for privacy, security, or controlling access. For example, in universities, a proxy server may block access to certain websites by checking all traffic and denying requests for restricted sites.

---

# What is a VPN?

A **VPN (Virtual Private Network)** is a service that creates a secure, encrypted connection between your device and the internet. It routes your internet traffic through a VPN server, which hides your IP address and encrypts your data, making it unreadable to outsiders.

### Key Points:

1. **Encryption**:
   - VPNs encrypt your data, which protects your information from being read by your Internet Service Provider (ISP), government agencies, or any third parties.

2. **Privacy**:
   - By masking your IP address and encrypting your data, VPNs help maintain your online privacy and anonymity.

3. **Secure Access**:
   - VPNs allow you to securely access restricted or geo-blocked content by making it appear as though you are accessing the internet from a different location.

4. **Protection on Public Networks**:
   - VPNs are particularly useful on public Wi-Fi networks, where they protect your data from potential interception by hackers.

---

## Difference Between VPN and Proxy

1. **Encryption**:
   - **VPN**: Encrypts your internet traffic, making it secure from eavesdroppers, including your ISP and government agencies.
   - **Proxy**: Does not encrypt your traffic. Your data is visible to your ISP and other entities.

2. **Privacy**:
   - **VPN**: Provides enhanced privacy by hiding your IP address and encrypting your data.
   - **Proxy**: Hides your IP address but does not provide encryption. Your data can still be intercepted and read.

3. **Scope of Protection**:
   - **VPN**: Secures all your internet traffic, regardless of the application or website you are using.
   - **Proxy**: Typically only affects the traffic of specific applications or browsers configured to use the proxy.

4. **Usage**:
   - **VPN**: Suitable for comprehensive privacy and security, particularly when using public Wi-Fi or accessing sensitive information.
   - **Proxy**: Often used for bypassing content restrictions or accessing blocked websites, but not suitable for secure, encrypted communication.

---

### Interview-Friendly Explanation:

**Q**: _What is a VPN, and how does it differ from a proxy?_  
**A**: A VPN (Virtual Private Network) creates a secure, encrypted connection between your device and the internet, protecting your data from being read by your ISP or third parties. It also hides your IP address and allows you to access restricted content securely. In contrast, a proxy server acts as an intermediary that hides your IP address but does not encrypt your traffic, meaning your data can still be accessed by your ISP or other entities.

---

# Client-Server Architecture

**Client-Server Architecture** is a model for designing networked applications where the workload is divided between clients and servers. It is a fundamental concept in both backend engineering and the broader internet ecosystem.

## Components

1. **Client**:
   - **Definition**: The client is the end-user device or application that requests resources or services from the server. This can be a web browser, mobile app, or desktop application.
   - **Function**: Sends requests to the server and displays the server's responses to the user.

2. **Server**:
   - **Definition**: The server is a powerful computer or software application that provides resources, services, or data to clients. Servers can be dedicated machines or cloud-based systems.
   - **Function**: Receives and processes requests from clients, performs necessary operations, and sends responses back to clients.

## How It Works

1. **Request**:
   - The client sends a request to the server. For example, when you enter a URL in a web browser, the browser (client) sends a request to the web server.

2. **Processing**:
   - The server processes the request. This may involve querying a database, performing calculations, or retrieving data.

3. **Response**:
   - The server sends the response back to the client. This might be a web page, data, or an error message.

4. **Display**:
   - The client displays the response to the user. For example, the web browser renders the web page for you to view.

## Key Points in Client-Server Architecture

- **Scalability**: Servers can handle multiple clients simultaneously, allowing the system to scale with increased demand.
- **Centralization**: Servers centralize resources and services, making them easier to manage and maintain.
- **Security**: Servers can enforce security measures and control access to resources.
- **Maintenance**: Updates and maintenance are easier to manage since they are performed on the server rather than on each client.

## Common Interview Questions and Answers

1. **Q**: _What is Client-Server Architecture?_
   - **A**: Client-Server Architecture is a network model where client devices or applications request services or resources from a centralized server. The server processes these requests and returns the required data or services to the client.

2. **Q**: _What are the main components of a Client-Server system?_
   - **A**: The main components are the client (which requests services or data) and the server (which provides the requested services or data).

3. **Q**: _How does a Client-Server interaction work?_
   - **A**: The client sends a request to the server. The server processes the request, performs necessary operations, and sends a response back to the client, which then displays the result to the user.

4. **Q**: _What are some advantages of Client-Server Architecture?_
   - **A**: Advantages include scalability (handling multiple clients), centralization (easier management and updates), security (centralized control), and easier maintenance.

5. **Q**: _What is the difference between a client and a server?_
   - **A**: A client requests services or resources from a server, while the server provides these services or resources. Clients typically interact directly with users, while servers handle the processing and storage of data.

6. **Q**: _What is meant by "scalability" in the context of Client-Server Architecture?_
   - **A**: Scalability refers to the system's ability to handle an increasing number of clients or requests. A well-designed client-server system can manage more users or higher loads by upgrading the server or distributing the load.

7. **Q**: _How does Client-Server Architecture ensure security?_
   - **A**: Security is managed through authentication, authorization, and encryption on the server side. The server controls access to resources and ensures data is securely transmitted and stored.

8. **Q**: _What are some common types of servers in a Client-Server system?_
   - **A**: Common types of servers include web servers (serve web pages), database servers (store and manage databases), and application servers (run applications and process data).

---

# Reverse Proxy: Your Invisible Guardian

A **reverse proxy** is a server that sits between client devices and the backend servers they want to access. Unlike a traditional proxy, which acts on behalf of the client, a reverse proxy acts on behalf of the server. It manages and directs incoming client requests to one or more backend servers.

Technically, **Reverse Proxy** is set up by the server in such a way that all the requests before reaching the backend server, goes through the **Reverse Proxy server** which further verifies that there is no malicious things in the request and it also verifies that whether the person has been sending multiple requests in a specific time period and if the request passes all the verification tests after then it is sent to the backend server, **So basically we use Reverse Proxy mainly for Rate Limiting**.

## How a Reverse Proxy Works

1. **Client Request**:
   - A client makes a request to access a website or service.

2. **Reverse Proxy Handling**:
   - The request is first directed to the reverse proxy server instead of directly to the backend server.

3. **Request Forwarding**:
   - The reverse proxy evaluates the request and forwards it to the appropriate backend server.

4. **Backend Server Response**:
   - The backend server processes the request and sends the response back to the reverse proxy.

5. **Response to Client**:
   - The reverse proxy then sends the response back to the client.

## Benefits of Using a Reverse Proxy

1. **Load Balancing**:
   - Distributes incoming traffic across multiple backend servers to balance the load and ensure no single server is overwhelmed.

2. **Enhanced Security**:
   - Acts as an additional layer of security by hiding the backend server’s IP addresses and protecting against direct attacks.

3. **Caching**:
   - Caches frequently requested content to improve performance and reduce the load on backend servers.

4. **SSL Termination**:
   - Handles SSL/TLS encryption and decryption, offloading this resource-intensive task from the backend servers.

5. **Compression**:
   - Compresses outgoing data to reduce bandwidth usage and improve load times for clients.

6. **Request Filtering**:
   - Can filter and block harmful or unwanted requests before they reach the backend servers.

7. **Application Firewall**:
   - Provides additional protection by filtering requests based on specific rules and security policies.

## Common Use Cases

- **Web Hosting**: Directs requests to multiple web servers based on load, user location, or content type.
- **API Management**: Routes API requests to different services and handles authentication and rate limiting.
- **Content Delivery**: Caches and delivers static content to improve performance and reduce server load.

## Interview-Friendly Explanation

**Q**: _What is a reverse proxy, and what are its benefits?_  
**A**: A reverse proxy is a server that sits between clients and backend servers. It forwards client requests to the appropriate backend server and then sends the server’s response back to the client. The benefits include load balancing (distributing traffic across multiple servers), enhanced security (hiding backend server IPs), caching (improving performance), SSL termination (handling encryption), and request filtering (protecting against harmful requests).

---

# Normal Proxy vs. Reverse Proxy

## Normal Proxy

- **Who It Represents**: The **client** (like your web browser).
- **Purpose**: Hides the client's IP address and makes requests to websites on behalf of the client.
- **Use Case**: Useful for privacy or accessing blocked content.

## Reverse Proxy

- **Who It Represents**: The **server** (like a website or application server).
- **Purpose**: Hides the server's IP address and handles requests from clients, then forwards them to backend servers.
- **Use Case**: Useful for load balancing, security, and caching on the server side.

---

In summary, a normal proxy acts on behalf of the client, while a reverse proxy acts on behalf of the server.






