<h1 align="center"> Cấu Hình Mạng Máy Tính - Cisco Packet Tracer <br/></h1>

<p align="center">
  <img width="90%" src="https://user-images.githubusercontent.com/91842746/196658865-aabe823f-5994-4b96-a9e8-af97098d9a7a.png" /></a>
</p>


# [**Table Of Content**](#table-of-content)
- [**Table Of Content**](#table-of-content)
- [**Introduction**](#introduction)
- [**Overview**](#overview)
- [**Content**](#content)
- [**Official Exam**](#official-exam)
- [**Document**](#document)
- [**Post Script**](#post-script)
- [**Our Team**](#our-team)
- [**Made with 💘 and Vietnamese <img src="https://cdn.britannica.com/41/4041-004-D051B135/Flag-Vietnam.jpg" width="30">**](#made-with--and-vietnamese-)

##

# [**Đề Bài**]
A. Scenarior: Implement network for Company BKACAD with 2 SITEs connect to the INTERNET. The company uses both IPv4 and IPv6 for the network, detail as follow:

- SITE1-LAN2 use only IPv4 address.
- SITE1-LAN1 use both IPv4 and IPv6 address (dual stack).
- Wan link use both IPv4 and IPv6 address (dual stack).
- SITE2-LAN3 use only IPv6 address
- Note: DNSv4 assign only IPv4 address, and DNSv6 assign only IPv6 address.

B. The tasks are performed by following parameters:
1. IP Address planning:
<p align="center">
  <img width="80%" src="https://user-images.githubusercontent.com/91842746/196716380-d0941424-d210-4cec-b1af-edd0dc933fc7.png" /></a>
</p>
 
2.Assign IP address, subnet mask, default gateway to the networking devices.
a. All routers and server are assigned IP address manually as following rule:
- Router interface : +1
- DHCP : +2
- WEB,MAIL : +3
- DNS: +4
- TFTP : +5, PC1 : +11, PC2 : +12; PC3 : +13; PC4 : +14
- Note:  PC5, PC6, PC7, PC8 : assigned IP address by DHCP server.

Ex: In the subnetwork: 192.168.1.128/25. (there are DHCP, PC5)
Router's interface : 192.168.1.129   (128+1).
DHCP server :192.168.1.130           (128+2).
PC4 client : 192.168.1.142           (128+14)
 

3.Basic router configuration:
- Overall requirements: all network segments in the network diagram can connect to each other (example: ping and tranceroute work for to reach all devices and PCs); users can telnet to get access to router CLI.

a) Router name, MOTD banner and descriptions
<p align="center">
  <img width="80%" src="https://user-images.githubusercontent.com/91842746/196717390-173ffddc-5a43-44bb-9d9e-fe446c5f1c7f.png" /></a>
</p>

b) Password:
+ The console are protected by clear text password (Unencrypted), password= cisco@console”
+ All VTY lines (0 – 4) are protected by clear text password (Unencrypted), password= ”cisco@vty”
+ Set the secret password to enter privileged mode, password= “cisco@enable”.

4.Configuring the SERVERS:

a. DHCP server:

### DHCP for LAN2 :
- PoolName: serverPool
- Start IP address: +10.
- Maximum number of user: 100

### DHCP for LAN 4 :
- PoolName: serverPool
- Start IP address: +50
- Maximum number of user: 150


b. Enable TFTP server. Backup routers’ configuration with the file name: R1-confg, R2-confg.

c. MAIL:
   ### Mail server:
   + Domain name: bkacad.com.
   + Add username/password: pc1/cisco and pc3/cisco
   + PC1 Mail client:

  ### Name: PC1
  + Mail address: pc1@bkacad.com
  + Incoming and outgoing mail server: bkacad.com
  + User pc1, pass cisco

  ### PC3 Mail client:
  + Name: PC3
  + Mail address: pc3@bkacad.com
  + Incoming and outgoing mail server:bkacad.com
  + User pc3, pass cisco

5.Test.
- From PCs, check connectivity with web server bkacad.com;cisco.com

- From PC1, Note: send mail from PC1 to PC3 and check the result.

##


# [**CHIA IPV4 theo Host**](#Chia-ipv4)
<p align="center">
  <img width="80%" src="https://user-images.githubusercontent.com/91842746/196668952-6abbfd06-fee1-4898-80fb-3e2bec5e51a7.png" /></a>
</p>

<p align="center">
  <img width="80%" src="https://user-images.githubusercontent.com/91842746/196666290-dc8e56fe-dbdc-4f0f-a5a0-348571178a9d.png" /></a>
</p>


# [**CẤU HÌNH ROUTER**](#router)
## Router 1




