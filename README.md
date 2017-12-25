# WiShark
Simulating the packet capturing and analysis operations of Wireshark using C#

## INTRODUCTION
Wireshark is the world’s foremost and widely-used network protocol analyzer. It is used for network troubleshooting, analysis, software and communications protocol development, and education.

## PROJECT DESCRIPTION 
The project was built with the purpose of simulating the packet capturing and analysis operations of Wireshark. C# was used to build both the backend and the project’s Graphical User Interface(GUI). The project’s features include:
-	Selecting the desired Capture Network (Ethernet, WIFI, ...etc.).
-	Controlling the Start and Stop sniffing.
-	Showing the user main details of the packets in a table.
-	If the user clicks on a packet, it will show him a detailed view for UDP or TCP protocols.
-	If the user clicks on a packet, it will show him hex view
-	The captured packets can be filtered based on the main columns of the table

## Prerequisites
- Net 4.0 and WinPcap should be installed for proper execution of the program.
  -	You can download WinPcap from here https://www.winpcap.org/install/
  -	You can download .Net 4.0 from here https://www.microsoft.com/en-us/download/details.aspx?id=17851
## Code Build
  ### 1.  Graphical User Interface (GUI)
  To design the User Interface we used two forms, one for the user’s greeting page which contains a list of devices for the user to     choose from to determine which one he would like to start capturing packets.
  
  ![Alt text](https://user-images.githubusercontent.com/26356497/34335094-db57a30c-e954-11e7-9396-5f5235de23bf.PNG)
 
The other form represents the page where the packets captured, and their information are displayed along with the controlling properties that are allowed for the user.

![Alt text](https://user-images.githubusercontent.com/26356497/34335095-db7c2ff6-e954-11e7-8913-36379bbdd0d2.PNG)
 
### 2.  Backend Structure
The phases for building the backend structure of the application were as following:
1.	Determining the needed packages such as PacketDotNet, SharpPcap.WinPcap…etc. 
2.	Making the devices global
3.	Building a function for getting devices
4.	Setting up hex viewer
5.	Setting up the function for receiving packet 
6.	Determining packet data name
7.	Retrieving data from packets
8.	Determining IP protocol
9.	Displaying packet information in readable format for the user
10.	Stop and Start functions for the user to be able to control the capturing process

## Features
-	Controlling Start and Stop sniffing
 
 ![Alt text](https://user-images.githubusercontent.com/26356497/34335092-d9f6ea90-e954-11e7-9811-e9bffacca1b3.PNG)

-	Showing main details of packets in a table
 
 ![Alt text](https://user-images.githubusercontent.com/26356497/34335096-db9ebff8-e954-11e7-970f-a7db7e896a26.PNG)

-	Detailed view for UDP and TCP protocols
 
 ![Alt text](https://user-images.githubusercontent.com/26356497/34335101-e5ad4d70-e954-11e7-86e0-db7e54741016.PNG)
 ![Alt text](https://user-images.githubusercontent.com/26356497/34335103-e6163a2e-e954-11e7-9a6c-e02ded430b9f.PNG)
 ![Alt text](https://user-images.githubusercontent.com/26356497/34335186-847c7098-e955-11e7-9d67-1b90167cf94c.PNG)
 ![Alt text](https://user-images.githubusercontent.com/26356497/34335187-84b73110-e955-11e7-95a4-32cf94ef6a0e.PNG)
 ![Alt text](https://user-images.githubusercontent.com/26356497/34335188-8525f8ac-e955-11e7-8f86-7cc8623b3468.PNG)
 

-	Hex view

![Alt text](https://user-images.githubusercontent.com/26356497/34335189-85f60998-e955-11e7-9ac5-76c219c2de3f.PNG)

-	Filtering Captured Packets based on the main columns of the table
 
 ![Alt text](https://user-images.githubusercontent.com/26356497/34335191-8a5b9a2a-e955-11e7-8dfc-df7c9ce55190.PNG)
 
-	Saving captured packets to file and loading captured packets from file

![Alt text](https://user-images.githubusercontent.com/26356497/34335192-8c2e951e-e955-11e7-87ab-ca707d5ce971.PNG)

- Shawing statistics
 
 ![Alt text](https://user-images.githubusercontent.com/26356497/34335196-8f340fb4-e955-11e7-9b16-e8586e8d924c.PNG)


