# Challenge Description:

<div align="justify">
  Alexis is a fictional cybersecurity company with thousands of employees. An attacker has gained unauthorized entry into its premises and has connected their laptop to an unused port on a switch. 
  The attacker now has access to the company’s internal networks. Within the internal network, there is a central server where critical proprietary data is stored. 
  In this capture, the attacker is attempting to collect SSH credentials that they can use to log into the central server.
</div>

## Tool Used:
Wireshark

## Questions:
1. What is the MAC address of the attacker?
2. What is the type of attack which is taking place that allows the attacker to listen in on conversations between the central server and another host?
3. What is the file which was downloaded from the central server?
4. What department does Borden Danilevich work in?
5. What is the SSH password of the Domain Administrator?

## Answers:
1. 08:00:27:3d:27:5d <br><br>
To find the MAC address of the attacker, type "ssh" in the display filter of Wireshark. Then, on the main screen of Wireshark, I checked the first packet showing on the screen (packet 765). I examined the Ethernet details to find the answer.

<div align= "center">
  <img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/a40f3176-6462-4969-86e8-7608b790bfd2" alt="c1">
</div><br>
   
2. man in the middle attack  <br>
<div align="justify">
  The attacker executed a man-in-the-middle (MitM) attack, a type of cybersecurity breach where a malicious actor intercepts and potentially alters communication between two parties without their knowledge or consent. By positioning themselves between the two parties, the attacker relays and possibly manipulates the messages exchanged between them, effectively controlling the flow of information.
</div><br>

3. Alevis_Employee_Information_Chart.csv <br><br>
To identify the file downloaded from the central server, I start by analyzing the protocols used in the PCAP file. To do this, I navigate to the 'Statistics' section in Wireshark and then select 'Protocol Hierarchy', which provides a comprehensive overview of all the protocols in use.
<div align="center">
  <img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/300f2e1b-0eb5-4112-b15a-b4f5906ca415" alt="Image">
</div><br>

Next, I examine the 'Transmission Control Protocol' section, where I find that the PCAP file has captured 'File Transfer Protocol' (FTP) traffic. To isolate this traffic, I return to Wireshark's main screen and apply a display filter by typing 'ftp', which helps me focus on the relevant packets.  <br><br>
<div align="center">
<img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/69c8fe55-4948-42fe-b4c6-9008f4cd6e69">
</div><br>
I select the first result, which corresponds to packet 550, by right-clicking on it. Then, I choose the 'Follow TCP Stream' option from the context menu, which allows me to examine the contents of the TCP connection in detail. <br><br>
<div align="center">
<img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/5583d07e-14b6-497b-8a5a-78ba6991d835">
</div><br>

4. Sales <br><br>
To find the answer to the question 'What department does Borden Danilevich work in?'. First, I enter the display filter 'ftp' to isolate the FTP traffic. Next, I select 'Follow TCP Stream' to examine the contents of the TCP connection. In the bottom-right corner of the Wireshark window, I navigate to the 'Stream' section and select stream 1, which displays the contents of the CSV file. As a final step, I use the 'Find' function, located in the bottom-left corner, and type 'Borden' to quickly locate his information within the file.
<div align="center">
<img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/d50477b1-dc7b-4bee-88c3-b33003a574d7">
</div><br>

5. gMR<4eXf]e6W <br><br>
To easily find the SSH password of the Domain Administrator. First, I enter the display filter 'ftp' to isolate the FTP traffic. Next, I select 'Follow TCP Stream' to examine the contents of the TCP connection. Then, I use the 'Find' function and search for the keyword 'admin', which quickly takes me to the relevant section of the captured data, revealing the SSH password of the Domain Administrator.
<div align="center">
<img src="https://github.com/Gepzuu/BTJA-Course-Capstone/assets/92858147/d8138a70-a8c1-4bd4-bb95-b065155f1a07">
</div><br>


   





