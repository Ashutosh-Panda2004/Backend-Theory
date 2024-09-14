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



