### EXPERIMENT -07 CONFIGURING NETWORK SERVER FOR CONNECTING GATEWAY AND END NODE 
 
## Aim: 
To  configure the Network server and end device for transferring data on the network
## Components required: 
End node stm 32 development kit , Dragino LPS8, Network server 

## Theory :
When working with sensitive applications or files, saving progress on your local device is a start, but what if you lose access to your device? Network servers address this problem by hosting the files and programs most pertinent to the network and enabling access for consistent, real-time use. 

As a result, personnel or network clients can instantly access important data or tools while also facilitating collaboration between users. Multiple users can make changes to the same program or document for continued development over the course of a project. Via a secure login, remote users can connect to the home network.
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/59db9b76-ddd5-4d6a-9075-8db233f5e479)


In the above graphic, the circle represents an organization network where a network server facilitates collaboration and file sharing between network clients (devices).

 The role of a network server, then, is to provide users with a set of services and access to resources on the network. These features include:

Permissioned access and log-ins for network users Gateway access to the Internet for an organization Centralized location for network resources  Shared access to devices on the network like a printer or a scanner Hosts multi-user apps like email servers, web applications, or CRM

## Procedure :

 1. login to the network server using login link  https://iot.saveetha.in/
 2. Click on the nework server as shown blow
    
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1bd434ca-1426-4102-8384-94473483543e)
 3. Click on the add gateway 
 
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/47c2e08d-6598-4437-8b07-f213d6f3b8ac)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/e62ff028-99bc-485e-9808-fbb6e124f8b2)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/a2e3ae58-6402-49e8-8f96-679059c1842c)
4. Click on the lora options , lora - frequency plan 

5. Click on channels and create a new channel after which you can add a new end device
   
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1fb72be5-e48d-4cde-a329-0cfb0d29070f)

6. Add the attributes in the end device as  shown below 

 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/00bff30b-42fc-42d5-9540-285d270e41cb)
 
7.Using AT commands configure end device in serial port utility
AT Commands to set initially (Mandatory)
 AT+FDR // To do factory data reset
 AT+NJM=1 // To set OTAA mode
 AT+ADR=1 // To enable the ADR
 AT+TDC=600000 // To set the default sampling interval as 10 minutes
(Should not give below 5 minutes)
 AT+CLASS=C // To set class C
 AT+DEUI=XX XX XX XX XX XX XX XX // To set Device EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX // To set APP EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX //
To set APP Key
 ATZ // To take effective action on below settings (As like saving)



## OUTPUT 
<img width="1920" height="1080" alt="Screenshot 2025-11-20 230242" src="https://github.com/user-attachments/assets/24f374db-a280-412f-a42f-98b3318a6d33" />
<img width="912" height="726" alt="image" src="https://github.com/user-attachments/assets/9121499e-b20b-4c33-9941-d9b996b8c35f" />
<img width="938" height="702" alt="image" src="https://github.com/user-attachments/assets/9f56d978-4cd2-44b7-a7ee-ad9a825f6c93" />
<img width="1920" height="1080" alt="Screenshot 2025-11-20 230932" src="https://github.com/user-attachments/assets/af57f4e9-7b2c-49a0-b646-940361aef035" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f927e40b-a42f-41c6-8732-db69cf492f50" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e82a135b-84d6-4689-96a4-ad50de29d0eb" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/add57c67-54cf-482d-843f-934a9b763a9e" />

<img width="1920" height="1080" alt="Screenshot 2025-11-17 141659" src="https://github.com/user-attachments/assets/fe32484e-b449-4d11-8415-ba1826abb165" />

<img width="1920" height="1080" alt="Screenshot 2025-11-17 141725" src="https://github.com/user-attachments/assets/c4cc336f-460e-46dc-81dd-cd86a698d5ad" />

<img width="1920" height="1080" alt="Screenshot 2025-11-17 141745" src="https://github.com/user-attachments/assets/e728c8f3-f1b0-4a93-91b9-74fe5b719b43" />

<img width="1920" height="1080" alt="Screenshot 2025-11-17 141807" src="https://github.com/user-attachments/assets/b308253a-407f-47a0-9174-ef8b36c3131b" />

<img width="1920" height="1080" alt="Screenshot 2025-11-17 141840" src="https://github.com/user-attachments/assets/5a8ae347-e13e-42a0-aae3-26ea612aa859" />

<img width="1920" height="1080" alt="Screenshot 2025-11-17 141900" src="https://github.com/user-attachments/assets/6c73630d-b887-416f-a0ae-6a26d46bab55" />

<img width="1920" height="1080" alt="Screenshot 2025-11-17 141920" src="https://github.com/user-attachments/assets/b2984900-82bf-4f35-bda1-7c5a7c574c28" />


<img width="1920" height="1080" alt="Screenshot 2025-11-17 141948" src="https://github.com/user-attachments/assets/e4159c27-02cc-418d-b914-5252e1a777ef" />

















## Result: 

  The Network server and end device for transferring data on the network has been accomplished.
