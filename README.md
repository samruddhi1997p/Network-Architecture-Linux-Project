TELE5331 Spring 2020
```Linux Project```

``Project 3``

Now that you are well versed with various protocols, you are ready to take up this big
undertaking: act as the network engineer for your company! A good engineer comes up with a
solution considering all factors that are required for the project.
Your goal is to come up with the best possible solution that is robust, secure, dynamic and
intelligent for the given scenario.

Discuss requirements with your team and come up with a design that is feasible taking into
account the problem statement, resources and the deadline. Once approved by all team
members, implement the elements of the project individually and finally, integrate the
elements to complete the solution. The architecture of the project looks like this:


1. DNS

Your first task is to build a DNS implementation for a start-up company in the city of
Boston. As the engineer, you’re expected to implement a DNS server according to the
specific requirements given below
Naming Get a domain name of your choice for the start---up
Addressing IPv4 and IPv6 address for your organization
DNS Servers Configure name servers to handle queries for your domain
Documentation Document the details for future users

Guidelines

1. Assign a set of IPs (IPv4 and IPv6) that must be used for this project

2. You may use one of the following DNS servers: BIND, Posadis, PowerDNS

3. Create any 5 DNS records

4. Use IPv4 and IPv6 addresses in your implementation of records

5. Create reverse domain records addr.arpa and ipv6.arpa for the addresses you are
using

6. Configure a Master DNS server as well as a Slave DNS server, the Slave DNS should
automatically update with Master DNS server

7. Show the testing, along with the test plan and provide example of your
implementation

8. When you work/design your project remember that you must give a demo. Plan
accordingly


2. DHCP

The next task is to build a DHCP implementation your company. As the engineer, you’re
expected to implement a DNS server according to the specific requirements given below

Scope

A full range of IP addresses that can be leased from a DHCP server.
Address Pool The IP addresses in a scope that are available for lease.

Exclusion

Range

Address in the scope that are excluded from leasing. Excluded addresses are
normally used to give hardware devices, such as routers, a static IP address.

Reservation

A means for assigning a permanent IP address to a client, server, or hardware
device. Reservations are typically made for servers or hardware devices that
need a static IP address.

Lease The amount of time that a client may use an IP address before the client must re---
lease the IP address or request another one.

Guidelines

1. Assign IPv4 and IPv6 (unicast local) addresses to users dynamically as they enter
your company network

2. Show reserved IP addresses for particular machines

3. You may use ISC-DHCP or other DHCP server of your choice

4. Show the testing, mention the test plan and provide example of your
implementation

5. When you work/design your project remember that you must give a demo. Plan
accordingly


3. WEB SERVER & FIREWALL

Configure a web server for your company and secure it from external attacks. You must
be able to access the webserver using the domain name, IPv4 address and IPv6 address.
How can this be practically implemented in your Linux machine? What do you think is
the simplest way to secure your network from external networks attacks? Considering
that you don't have much funding to buy more security devices, how do you think you
can secure your server? There are different ways by which we can secure a server for
the above scenario. For example, it can be IP filtering, protocol filtering, etc. Make your
network as much secure as possible.

Guidelines

1. Use only command line tools and packages

2. Provide all the commands that you have used and give a brief description in one line

3. Provide the changes you have made to the files/folders for configuring the
webserver as well as the firewall. Also, create a basic web page to be served by this
web server.

4. Make this page accessible to the clients in your network using a web browser

5. Make your server the most secured one in all possible ways

6. Show the testing, mention the test plan and provide example of your
implementation

7. When you work/design your project, remember that you must give a demo. Plan
accordingly.


4. BACKUP

Isn’t it always better to design a robust system? When there is a group of people
working on a server, there is a possibility that the server might crash because of
increase in usage or because of the heavy- duty processes running on the servers. The
best way is to systematically create a backup of every day’s work from the current
server to a different server. Your task is to create a backup server that fulfills the
following requirements:

1. Automate the process of backing up the data such that it backs up periodically with
a unique timestamp to indicate the latest update

2. The backup file should be zipped and sent to a different server

3. Describe briefly about how you backup automatically and how file transfer is made

4. Also provide the commands and configurations for sending the zipped file to a
different location

5. Mention which protocol you are using to complete this task

6. Show the testing, mention the test plan and provide example of your
implementation

7. When you work/design your project remember that you must give a demo. Plan
accordingly

``Bonus``

1. ARP SPOOFING

The Address Resolution Protocol (ARP) is a telecommunication protocol used for
resolution of Internet layer addresses into link layer addresses, a critical function in
computer networks.
To earn these bonus points, you must implement a malicious user in your network
which hosts its own webserver. This malicious user is going to poison the ARP entry for
original web-server in the client’s ARP cache and once client sends a request to the IP
address of the original webserver, the request will be received by the malicious user and
user will see a Hacked Web-Page. You may use Ettercap, Bettercap or any other tool of
your choice.

2. IPSec VPN TUNNEL

Implement IPSec VPN tunnels between two linux machines using openswan or
strongswan or any other tool of your choice

3. NFS

Implement NFS. There should be at least 2 clients (can be VMs on which other servers
are hosted) to whom the shared file would be available
Project Report
Report should include your detailed work and methodology not limiting to the
following

1. Behavior of the protocol

2. Signaling

3. Hierarchy

4. Commands used

5. Algorithm & Flow Chart

6. Testing

7. Working with an example (Integration)

8. Provide screenshots of various packets involved in each of your protocol using Wireshark

9. Future improvements

Project Demo

1. Every group will be responsible for preparing themselves for a demo and explaining the
details of the project.

2. Demonstrate the functionality of each protocol and integration of all the parts
mentioned above.

3. Summary of the Demo: The DHCP server should be able to lease IP to clients; the
client should be able to access the web page hosted by the web browser by resolving its
IP from the DNS, and later the Firewall should be able to block the client; the client must
also be able to receive backup files from the backup server.