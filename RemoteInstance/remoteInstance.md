# Connecting to a remote instance via Neo Desktop

How to install and configure your local Neo4j sandbox instance.

- Download and install the Neo4j desktop application (https://neo4j.com/download/)

## Setting up Neo4j Desktop to a remote connection

- Open Neo Desktop
- If required create a new project
![Step1](../SandboxSetup/images/step1.PNG)
- Create a New Graph Database<br>
![Step2](./SandboxSetup/images/step2.PNG)<br>
     - Select `Connect to Remote  Graph`
     - Enter the name for the connection
     - Enter the bolt address
     :bulb: you do not need to include the port information.  `bolt://<DNS name` is enough<br>
     ![Step3](images/step3.png)
     - Select either `Username/password` or `Kerberos`<br>
     ![Step4](images/step4.png)
     - Enter the required credentials<br>
     ![Step4](images/step5.png)<br>
     :bulb: Select `Use encryped connection` only if you have a secure https connection in place<br>
     - Select `Connect`
 - ![Step6](images/step6.png)<br>
 Select Start to connect to the remote instance

 **NOTE** Start and Stop in the context of remote servers **DOES NOT** stop and start the remote services; you are simply opening a connection to the remote service.


 ### Note on plug-in
 Plug-ins need to be installed manually on the remote server, there is no means remotely deploy and manage these via the neo desktop

 