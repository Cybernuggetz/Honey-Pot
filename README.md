# HONEYPOT

## Objective

The Honey Pot Lab project aims to create a virtual control environment to simulate attacks that could potentially harm the company. As malicious actors grow increasingly sophisticated, many zero-day exploits not yet integrated into Threat Intelligence Feeds can bypass existing security configurations and cause operational damage. The lab captures live traffic from malicious actors and feeds it into the company’s Threat Intelligence system, enabling updates to security configurations to include previously unknown threats, thereby strengthening the company’s security posture. Additionally, the lab provides personalized configurations to identify and mitigate threats specifically targeting the company, neutralizing them before they can materialize.

### Skills Learned


- Creation of cloud virtual machine and deployment. 
- Windows log ingesting into Azure cloud.
- Ability to generate and recognize attack signatures and patterns.
- Usage of Kql to query the ingested log.
- Creation of Watchlsit to resolve attacker IP to countryname.
- Development of critical thinking and problem-solving skills in cybersecurity.
- Visualisation of log in a map and chart.

### Tools Used


- Security Information and Event Management (SIEM) system for log ingestion and analysis.
- Usage of remote desktop client tool to access the virtual machine.
- Microsoft Sentinel workbook to visualise the IP to country of location.

## Steps

*Step 1:
After logging into the Micrososft Azure homepage, the below interface was displayed. From, any needed tool can be choosen.

<img width="1366" height="768" alt="Screenshot From 2025-08-01 10-19-40" src="https://github.com/user-attachments/assets/abc92eda-d81f-4bd6-8168-762b63d3a275" />

*Image 1: Network Diagram* Azure home page <br>


*Step 2:
In the Azure search bar, I searched the resources group, and create a resource group called Cyber_Organisation. The resources group is like the organisation or company name which every tools used are ascribed to.

<img width="1366" height="768" alt="Screenshot From 2025-08-01 10-24-18" src="https://github.com/user-attachments/assets/f758dc1e-6377-4123-af7a-a2385c99d600" />

*Image 2: The resource group page<br>


*Step 3: 

Creation of Virtual Network. Through Azure search bar, the virtual network page can be assesed and this will assign and manage Ip address to machines under the network. The virtual network is tied to the resources group. 

<img width="1366" height="768" alt="Screenshot From 2025-08-01 10-26-37" src="https://github.com/user-attachments/assets/b2ed388a-adf5-4542-905d-22bdeef5dde4" />

*Image 3: virtual network page<br>


*step 4:
Creation of virtual machine. virtual machine is created to disguise as a real machine with a little bit of exposure to the wider world, on the network thereby luring attackers to attack the machines. The machine is configured to open certain port like ssh to facilitate remote access and then power on.

<img width="1366" height="768" alt="Screenshot From 2025-08-01 10-31-03" src="https://github.com/user-attachments/assets/5e57f781-01fa-4737-800f-0ef2abe534ab" />

*Image 4: Virtual machine<br>

*Step 5:
Through the use of allowed tunnel, the virtual machine is access by the local system

 <img width="1366" height="768" alt="Screenshot From 2025-08-01 15-33-52" src="https://github.com/user-attachments/assets/45f51831-99bd-460b-a198-a3b586794b5f" />

*Image 5: virtual machine laoding on the local system<br>

 
*Step 6: 
Log analytics workspace is created on the Azure to collect, store, analyse and visualise log data from the virtual machine.

<img width="1366" height="768" alt="Screenshot From 2025-08-01 12-06-10" src="https://github.com/user-attachments/assets/cefd28b6-7a2e-4bb4-93dd-9eb496b2e69c" />

*Image 6: Azure log analytics workspace<br>


*Step 7:
Through the Azure seach bar Microsoft sentinel is added to the resource group giving visualisation capability to the group.


<img width="1366" height="768" alt="Screenshot From 2025-08-01 12-42-19" src="https://github.com/user-attachments/assets/fa5c6dea-a722-4839-9799-92557dbae5cf" />

*Image 7: Microsoft sentinel 


*Step 8:
On Sentinel, the Content hub is accessed and Window Security Event is installed which comes with AMA connector, responsible for forwading window logs to log analytics

<img width="1366" height="768" alt="Screenshot From 2025-08-01 12-46-42" src="https://github.com/user-attachments/assets/ed22f194-40b0-4f81-804c-9a012c5a595a" />

*Image 8: Content hub



