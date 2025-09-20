# Ex. No: 6 Identifying MAC and IP Addresses Using Packet Tracer
# Date: 20-09-2025
________________________________________
# Objective
To use Cisco Packet Tracer simulation mode to capture and analyze MAC and IP address information for both local and remote network communication.
________________________________________
# Apparatus/Tools Required
•	Cisco Packet Tracer<br>
•	Pre-configured network topology (as provided in the activity file)<br>
•	PCs, switches, router, hub, and wireless access point (as per given setup)<br>
________________________________________
# Network Topology Diagram
# Description:
•	The topology contains a local network (172.16.31.0/24) connected to a remote network (10.10.10.0/24) via a router.<br>
•	Devices include PCs, switches, hub, and wireless AP.<br>
(Insert screenshot of your Packet Tracer setup here)<br>
________________________________________
# IP Addressing Table
(Example – actual values from simulation)<br>
Device	IPv4 Address	Subnet Mask	MAC Address<br>
PC-A	172.16.31.5	255.255.255.0	00D0:D311:C788<br>
PC-B	172.16.31.2	255.255.255.0	000C:85CC:1DA7<br>
Router (G0/0)	172.16.31.1	255.255.255.0	00D0:BA8E:741A<br>
PC-Remote	10.10.10.2	255.255.255.0	00D0:588C:2401<br>
________________________________________
# Procedure
# Part 1: Local Network Communication
1.	Click PC-A (172.16.31.5) and open the Command Prompt.<br>
2.	Enter ping 172.16.31.2.<br>
3.	Switch to Simulation Mode and repeat the ping.<br>
4.	When the PDU appears, click it and record: Destination MAC, Source MAC, Source IP, Destination IP, and the device name.<br>
5.	Use Capture/Forward to follow the PDU through the network until it reaches PC-B.<br>
6.	Record the information in a table.<br>
7.	Repeat the above process for:<br>
o	Ping from 172.16.31.3 to 172.16.31.2<br>
o	Ping from 172.16.31.5 to 172.16.31.4<br>
Part 2: Remote Network Communication<br>
1.	From PC-A (172.16.31.5), enter ping 10.10.10.2.<br>
2.	Switch to Simulation Mode and repeat the ping.<br>
3.	When the PDU appears, note the Destination MAC, Source MAC, Source IP, and Destination IP.<br>
4.	Follow the PDU step-by-step until it reaches the remote PC.<br>
5.	Observe how MAC addresses change at the router while IP addresses remain constant end-to-end.<br>
________________________________________
# Example Data Recording Table
At Device	Dest. MAC	Src MAC	Src IPv4	Dest IPv4<br>
172.16.31.5	000C:85CC:1DA7	00D0:D311:C788	172.16.31.5	172.16.31.2<br>
Switch1	000C:85CC:1DA7	00D0:D311:C788	N/A	N/A<br>
172.16.31.2	00D0:D311:C788	000C:85CC:1DA7	172.16.31.2	172.16.31.5<br>
________________________________________
# Output (Screenshots)
•	PDU details for local communication<br>
<img width="1919" height="1016" alt="Screenshot 2025-09-20 141112" src="https://github.com/user-attachments/assets/ea7f3d4f-dd38-4a12-a86f-bac91f3da47c" />
<img width="1919" height="1008" alt="Screenshot 2025-09-20 141055" src="https://github.com/user-attachments/assets/66d0e46a-e56b-4bb2-9c2f-71082ac83074" />
<img width="1919" height="1012" alt="Screenshot 2025-09-20 141041" src="https://github.com/user-attachments/assets/7997077a-d0ef-47ac-b9a3-298e49f59a2e" />
<img width="1919" height="1016" alt="Screenshot 2025-09-20 141023" src="https://github.com/user-attachments/assets/7f2b61b9-e2be-44e5-8d1e-1f09251b6a6c" />

•	PDU details for remote communication<br>
<img width="1919" height="1012" alt="Screenshot 2025-09-20 141356" src="https://github.com/user-attachments/assets/667f7641-d86a-4110-9554-b452948f94f5" />
<img width="1919" height="1017" alt="Screenshot 2025-09-20 141342" src="https://github.com/user-attachments/assets/799d2056-f289-4e32-b00c-16c425e2ef51" />
<img width="1919" height="1016" alt="Screenshot 2025-09-20 141321" src="https://github.com/user-attachments/assets/7bac091d-6545-408f-8c90-fbc883407d24" />
<img width="1919" height="1015" alt="Screenshot 2025-09-20 141244" src="https://github.com/user-attachments/assets/43a72844-43be-4f56-9f4f-66ed7373dfac" />
<img width="1919" height="1011" alt="Screenshot 2025-09-20 141229" src="https://github.com/user-attachments/assets/c3d1a19b-321f-410c-a765-4f613aff8cf7" />
<img width="1919" height="1021" alt="Screenshot 2025-09-20 141412" src="https://github.com/user-attachments/assets/893cadb4-bfe9-4118-be27-bcdd5fe1faac" />

•	Tables showing MAC/IP changes through each device<br>
<img width="616" height="193" alt="Screenshot 2025-09-20 141517" src="https://github.com/user-attachments/assets/f8f6c152-5f0d-4fe7-b83b-de2fe4636f7c" />
<img width="622" height="141" alt="Screenshot 2025-09-20 141501" src="https://github.com/user-attachments/assets/ac0b680d-4ae6-45fc-8d5e-287f6a085289" />

________________________________________
# Result
Successfully captured and analyzed MAC and IP addresses for both local and remote communications. Verified that MAC addresses change at each hop while IP addresses remain constant from source to destination.

