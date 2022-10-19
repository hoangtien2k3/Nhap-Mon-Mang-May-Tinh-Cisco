<h1 align="center"> Cấu Hình Mạng Máy Tính - Cisco Packet Tracer <br/></h1>

<p align="center">
    <img src="https://user-images.githubusercontent.com/91842746/196658865-aabe823f-5994-4b96-a9e8-af97098d9a7a.png" width="1280" />
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
    <img src="https://user-images.githubusercontent.com/91842746/196716380-d0941424-d210-4cec-b1af-edd0dc933fc7.png" width="1200" />
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
 

3. Basic router configuration:
- Overall requirements: all network segments in the network diagram can connect to each other (example: ping and tranceroute work for to reach all devices and PCs); users can telnet to get access to router CLI.

![Screenshot 2022-10-19 211842](https://user-images.githubusercontent.com/91842746/196717390-173ffddc-5a43-44bb-9d9e-fe446c5f1c7f.png)



# [**CHIA IPV4 theo Host**](#Chia-ipv4)

<p align="center">
    <img src="https://user-images.githubusercontent.com/91842746/196668952-6abbfd06-fee1-4898-80fb-3e2bec5e51a7.png" width="1280" />
</p>

<p align="center">
    <img src="https://user-images.githubusercontent.com/91842746/196666290-dc8e56fe-dbdc-4f0f-a5a0-348571178a9d.png" width="1280" />
</p>



# [**CẤU HÌNH ROUTER**](#router)
- Router 1
![Screenshot 2022-10-19 174139](https://user-images.githubusercontent.com/91842746/196669684-d19d6276-e840-4ec1-b9b7-e8b2b376cbbc.png)
- Router 2
![Screenshot 2022-10-19 174408](https://user-images.githubusercontent.com/91842746/196670225-52067292-fc2c-4d89-ae8e-594227877df7.png)



