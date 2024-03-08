# Net Working


### **i. Network Devices :**

1. **Hub :**  
    A hub is a device that forms part of a network for transmitting information between devices, however, the information sent by a device is received by every other device whether it was intended for that device or not.
    
2. **Switch :**  
    A switch forms part of a network for transmitting information between devices, however, it only transmits information to the relevant device by using the MAC Address of that device.  
    \-Layer 2 Switch: Operates at the Data Link layer and transmits Packets using MAC Address.  
    \-Layer 3 Switch: Operates at both Data Link & Network layer and transmits Packets using IP and MAC Address.
    
3. **Router (Wireless/Wired) :**  
    A router is a device that sets up a separate wireless LAN for devices to connect to it, it serves the option for both wired and wireless connection.  
    ISP ──&gt; Router ──&gt;Devices
    
4. **WAP(Wireless Access Point) :**  
    Wireless Access Points are part of a Network and are used for the availability of Wireless networks at scale/ Extended availability in workplaces.  
    The general connection is set in the following way  
    ISP ──&gt; Modem/Router ──&gt; WAP ──&gt; Devices
    
5. **Firewalls :**  
    A firewall is a Network security system that filters a Network's Incoming and outgoing traffic based on allowing trusted traffic to enter and blocking the Untrusted.
    

### ii. Types Of Networks :

        1. PAN:A Personal Area Network is used for sharing small files via (Bluetooth, Infrared) or USB cable.
    
        2. LAN: The Local Area Network consists of devices located close to each other. Inside a LAN, multiple subnets can be created for the segregation of networks for relevant departments.
    
        3. VLAN: Virtual Local Area Network helps in maintaining multiple LANs at a time while managing cost. When multiple LANs are set so instead of deploying separate network switches and             cabling for each LAN, VLANs are set that logically partition the same switch for multiple LANs as a result of which traffic of all the LANs can be segregated and transmitted.
    
        4. WLAN: A Wireless Local Area Network is a LAN with wireless connectivity between devices.
    
        5. CAN: A Campus Area Network joins 2 or more LANs together, e.g. a University where Individual buildings having a LAN combine with others to form a CAN.
    
        6. MAN: Metropolitan Area Network is between different infrastructures in a city for sharing Information, the connectivity is via fiber cables.
    
        7. WAN: Wide Area Network comprises MANs, CANs, and LANs. It is over a large area such as countries.  
           Inside WAN there are LANs, Inside LANs, there are multiple Subnets.
    
        8. VPN: A Virtual Private Network can be considered a tunnel used for secure and encrypted communication between the client and a server.  
           Organizations use VPNs in a manner that their user connects with the VPN to connect to their server and network resources so secure communication is ensured.
     

### **iii. Routing Protocols :**

  1. **NAT :**  
      Network address translation is used for translating IP addresses from Public to Private and vice versa. Its use case is in the home networks when N number of devices are connected to   
      the Internet so their private IP which is inside the home network is not revealed publicly rather a Public IP is assigned to them from the Outer using NAT when they interact with the         Internet.  
      On the contrary, when the public IP brings a queried response back the NAT translates that to the Private IP for the device.
    

### **iv. OSI Model :**

The Open Systems Interconnection (OSI) Model is a conceptual framework for understanding Network Communication. It comprises of 7 Layers

  i.  Application Layer: Performs <mark>(</mark>**<mark>HTTP/FTP/SFTP/TFTP/SSH/DNS/SMTP)</mark>**  
  ii. Presentation Layer: Encrypts the Data to be sent via the request **<mark>(SSL/TLS)</mark>**  
  iii.Session Layer: For User's session creation **<mark>(NetBios)</mark>**  
  iv. Transport Layer: For data segmentation and Transmission protocol definition **<mark>(TCP/UDP)</mark>**  
  v.  Network Layer: Assigns **IP** addresses of source and destination to data packets being sent **<mark>(IP, ICMP)</mark>**  
  vi. Data Link Layer: Assigns MAC addresses for the data packets that are converted to frames **<mark>(MAC)</mark>**  
  vii.Physical Layer: Consists of the medium via which data will be taken to the final destination **<mark>(Ethernet, USB)</mark>**

**<mark>USE CASE :</mark>**  
BOB searches for www.facebook.com on the browser

  i) The application layer initiates an HTTP request consisting of Facebook.com at the browser level.

  ii) The presentation layer encrypts the request.

  iii) The session layer initiates, handles, and terminates the Facebook session for BOB.  
   **The above 3 layers perform at the browser level**

  iv) The transport layer segments the data and selects UDP/TCP as BOB is requesting to watch a live stream.

  v) Network Layer assigns IP addresses i.e. BOB's Public IP and Facebook server's Public IP for packet transmission.

  vi) The Data Link layer encapsulates data packets into frames including the MAC address of BOB's device and Facebook's server's source.

  vii) The physical layer Utilizes the medium set between Bob's location and Facebook's server.

### v. TCP/IP Model --&gt; TCP/IP Layer

  1 . Application Layer --&gt; (Application layer, Presentation Layer, Session Layer)  
  2. Transport Layer --&gt; Transport Layer  
  3. Internet Layer --&gt; Network Layer  
  4. Network Layer --&gt; Network Interface Layer

### vi. Protocols :

      1. Application Layer Protocols:
    

  a) **HTTP** :  
       Hypertext Transfer Protocol is fundamental to the web and is used for sending and receiving hypertext links.

  b) **HTTPS** :  
       Hypertext Transfer Protocol Secure is HTTP with an added security layer either via SSL or TLS for data encryption.

  c) **FTP** :  
      File Transfer Protocol is used for Transferring files from client to server so they can be accessed on the server.

  d) **SFTP**:  
      Secure File Transfer Protocol is a secure version of FTP as it encrypts the data during transmission as well as authenticates the sender and receiver.

  e) **TFTP**:  
      Trivial file transfer protocol is a form of FTP but it is only used in the local area network.

  f) **SSH** :  
      Secure Shell is used to connect to remote Linux machines over a secure channel.

**g) DNS :**
    The domain name system maps the name of a domain to the IP Address so the user can access the site just by entering the name of the site and not remembering the IP address associated 
    with it.

  1. Client &gt; Requests a Website &gt; Browser Cache  
    if the IP address is not found then
    
  2. Client &gt; Requests a Website &gt; Local DNS cache  
    if the IP address is not found then
    
  3. Client &gt; Requests a Website &gt; Host file  
    if the IP address is not found then
    
  4. Client &gt; Requests a Website &gt; ISP Recursive Domain Resolver  
    if the IP address is not found then
    
  5. Client &gt; Requests a Website &gt;  
      ISP Recursive Domain Resolver&gt;  
      Root Sever (Points to the TLD server) &gt;  
      Back to ISP Recursive Domain Resolver &gt;  
      TLD Server(Points to Authoritative Name Server) &gt;  
      Back to ISP Recursive Domain Resolver &gt;  
      Authoritative Name Server (Points to the IP Address for the requested website)
    
6. **DNS Records :**
    a) A Record :  
       Performs Name to IP resolution using IPV4 (32-bit)

    b) AAAA Record :  
       Performs Name to IP resolution using IPV6 (128-bit)

    c) Cname Record :  
       Canonical name record points a domain/subdomain name to another domain name.

    d) SOA Record :  
       The start of the Authority record configures and stores information about the administrator of a DNS zone.

    e) TXT Record :  
       TXT record performs an authentication check if the website is owned by the correct resource.

    f) MX Record :  
       Mail exchanger records point to the email server where the emails for the respective domain will be received. MTA queries the MX records for the site and DNS responds to MTA as to 
       which server to send email to.
       There are primary mail servers and secondary email servers as a backup to the primary.

    g) NS Record :  
       Provides the name of the Authoritative name server within a domain. NS record will list 2 nameservers, a primary and a secondary.

    h) SRV Record :  
       Service record points to the server as well as the port number for a service on a domain.

    i) PTR Record :  
       Pointer record points IP to name, used in email server to authenticate the email received from a domain in pointing to its respective IP address. It is a reverse DNS lookup.

  **h) DDNS :**  
      Unlike DNS where the IP issued by the DHCP is static and issues an error in DNS resolution if the IP changes. DDNS(Dynamic Domain Name System) assigns the dynamic IP which means if the       IP listed against a domain name changes, the new IP will be automatically assigned to the domain name for hassle-free access.

  **i) DHCP :**  
      Dynamic Host Configuration protocol assigns the IP to any device that connects to the network, the process takes place in a way that the new user when accesses the network makes a DHCP       request to the DHCP server which in turn offers the available IP address and settings to the user for a stated amount of time called a lease.  
      Upon selection from the user, the IP address is allocated to it.  
      In Intervals, the client requests the DHCP server for renewal of the IP lease else the lease will expire and the IP removed for that client.

**<mark>Automatic Private IP Addressing</mark>** is when the <mark>Windows client</mark> is unable to reach the DHCP server so the OS of the client automatically assigns a Private IP to it in the range :  
169.254.0.1 - 169.254.255.254

**j) SMTP :**  
Simple Mail Transfer Protocol is used for email communication between different user accounts.

    2. Presentation Layer Protocols:
**a) SSL :**  
Secure Socket Layer was previously majorly used for secure communication over the Internet via Applications and Browsers.  
  
b) TLS :  
Transport Layer Security is the newer and more secure version of SSL.

    3. Session Layer Protocol:

**a) NetBios :**  
Net Bios protocol is used to enable communication between devices inside a Local Area Network.

    4. Transport Layer Protocols:

**a) TCP :**  
Transmission control protocol is a connection-oriented protocol i.e. it ensures the establishment of a connection between both the client and server at first and then ensures sending all the packets of data.

**b) UDP :**  
User Datagram Protocol is not a connection-oriented protocol and is focused on sending the data packets at a faster speed than TCP, at times data packets get lost in the transmission.

    5. Network Layer Protocol:

**a) IP Addresses and Schemes :**

i. **IPV4** : 32-bit Numeric Address

ii. **IPV6:** 128-bit Hexa Decimal Address

iii. **Private IP :** 
      Assigned by DHCP to the devices inside the network, however, Private IPs are Inaccessible by the Internet and used internally.Assigned by the router to you.  
  
iv. **Public IP :**
     Accessible by the Internet and acts as an outer communicator medium on behalf of private IPs. The IPs are resolved from public to private and vice versa via NAT in the router.  
     Assigned by ISP

    6. Data Link Layer Protocol:

a) **MAC Address :**  
It is the hardware address of every device and is on the Network Interface attached to the device.IP address locates where the device on the Internet exists whereas MAC Address confirms what the device is. Multiple Network interfaces in a machine will result in multiple Mac addresses, however IP address can be changed but the MAC address remains constant.

    7. Physical Layer Standards:

**a) USB**  
**b) Ethernet Cables**

### vii. Ports :  
     Ports can be termed as virtual connection points where the connectivity initiates and ends. A use case is an application requesting something on the Internet, In response the router 
     receives the request containing the packet, which then Is sent to the respective device as a frame and the port hosting the application that made the request gets the info for the 
     application.  

### viii. Subnets, Gate Way :


a) **Subnet**: 
    SubNet or SubNetwork is a part of a larger network that can be assigned to a group to segregate its network traffic.  
  
  Types:  
  i. Public Subnet:
      Have Access to the Internet via a gateway, the resources in the Public subnet can access the Internet directly.  
  
  ii. Private Subnet:
      Does not Have Access to the Internet via a gateway, the resources in the Private subnet cannot access the Internet directly but rather need a NAT for it.  
  
b) **Gateway :** 
    A gateway is an Intermediary or middle resource that lets the data move from one network to a different network. Suppose there are 2 Networks A and B.  
    A consists of 4 nodes connected via a switch for communication in between, and B also consists of 4 nodes connected via a switch for communication.  
    A switch is used for their intercommunication, but if a node in Network A has to communicate with Network B, so it needs a default gateway for communication.  
    A router is a gateway.

### ix. Topologies :
  Topologies are patterns in which the nodes or machines in a system are connected. The most common Topologies are shown below:  
  
  a) Star Topology: It consists of a central hub to which all the nodes are connected.  
  b) Ring Topology: It consists of one node connected to 2 other nodes.  
  c) Mesh Topology: It consists of all nodes connected to each other in a network.  
  d) Bus Topology: It consists of all nodes connected to a central line/cable in between.  
  e) Tree Topology: It consists of a hybrid version of star and bus topology, in it multiple star topologies connect to a bus to form a topology.

![topologies](https://github.com/SaadatIrfan/Net-Working/assets/116474264/008c47ba-e840-44a4-b619-0b721af1bb25)



### x. Proxy & Reverse Proxy :
**a) Proxy:** 
     Proxy servers also termed as forward proxy is a server that is placed in front of the clients and is tasked to receive requests from the client for communicating with the     
     Internet on behalf of the clients and providing back to the clients what was received from the Internet. It is used as a shield to keep clients protected from outside threats.  
  
**b) Reverse Proxy:**
     Reverse proxy also termed as server-side proxy is placed in front of the actual servers to receive any incoming traffic coming from the clients and then request the 
     servers for it. It is used as a shield to protect servers from any potential threat request.

### xi. Virtualization and Cloud Computing :

**a) Virtualization:**
     Virtualization is a concept that was a state ahead of the conventional IT infrastructure. The conventional IT infrastructure consisted of having 1 server per 
     application hosting, which resulted in increased cost, covered area, and maintenance.  
     Virtualization involves hosting multiple applications on a single server by segmenting the resources of the server **per** application.  
  
    Types of Virtualization involve :  
  
  1)Storage Virtualization  
  2)Network Virtualization  
  3)Server Virtualization  
  4)Data Virtualization  
  
  
**b) Cloud Computing :**
     In virtualization, the cost of the IT infrastructure is reduced significantly. However, for the companies that are starting, are at mid-level, or at a large scale 
     that are considering cost as a major metric in their operations, cloud computing provided a leap forward. The companies that used complex on prime infrastructure now can use all the 
     resources in the cloud without having to deal with hardware maintenance or management.  
     It is a pay-as-you-go model, where you pay for the on-demand access to a computing resource rather than bearing the additional maintenance or purchasing cost.

### xii. Linux Commands and Jobs:

1. PING :  
    A ping request made by a client travels the network and retrieves the final destination information.
    ![ping](https://github.com/SaadatIrfan/Net-Working/assets/116474264/4bacb4e4-5ac3-4fa0-8d69-63c498ff667c)

    
2. Traceroute :  
    Traceroute is used to examine and look at the hops the client requests go through from one router to another and the final required destination. From the holistic picture, it can be 
    observed that the hop failed on which router.  
    It can be seen that the TTL(Time to Live) for a data packet is 30.  
    (tracert -h n abc.com) &gt; n in where TTl is set


    ![tracert](https://github.com/SaadatIrfan/Net-Working/assets/116474264/37704af4-7039-46b9-8ae2-a84421899cb3)

  
