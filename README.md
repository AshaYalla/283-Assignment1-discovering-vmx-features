# Assignment 1

** By Asha Yalla and Mounica Reddy Kandi **
>> This assignment was performed on Asha's GCP

### Asha's Contribution

Mounica and I reviewed the lecture’s video and followed his steps to discover vmx features in nested virtual machine. For this, I signed up to Google Cloud and created an instance of Intel Cascade Lake Architecture n2-standard-2. I’ve updated the configuration of the existing VM for the nested virtualization and installed the make module to run the prof’s files. Inserted the created modules into the kernel and displayed the features of the considered register. 

### Mounica's Contribution

Me and Asha worked together on this assignment. We checked the assignment details and reviewed the lecture recording on the assignment requirements. I retrieved the starter.c file and makefile from her GCP and added the additional structs and the definitions for the various capability info areas. I added the remaining reads of the msrs for each capability in the detect_vmx_features function and also added the calls to report_capability. I tried to perform testing on the newly created .ko file by running make followed by sudo insmod. 


## Steps Followed:

#### Step 1: Exported the current configuration of the files into the yaml file

<img width="468" alt="image" src="https://user-images.githubusercontent.com/99624135/200433279-669d8950-1bbd-4161-9898-a02f3974f13d.png">


#### Step 2: Updated the configuration file with details about nested virtualization

<img width="468" alt="image" src="https://user-images.githubusercontent.com/99624135/200433576-5674d6c9-59ab-479c-82d0-ce7d519e53ad.png">


#### Step 3: Updated the VM configuration

<img width="468" alt="image" src="https://user-images.githubusercontent.com/99624135/200433971-f94409fb-ea23-4ccc-9fe1-9a49e55ef545.png">


#### Step 4: Determining if VM virtualization is activated: getting anything other than 0 indicates the nested virtualization is activated.

<img width="468" alt="image" src="https://user-images.githubusercontent.com/99624135/200434312-094ff3d2-0b61-437d-8973-4e4b774e27ca.png">


#### Step 5: To print the vmx feature of the register and the make file, cloned the git repository using the professor's program.

<img width="468" alt="image" src="https://user-images.githubusercontent.com/99624135/200434601-33f2cd77-ada2-4595-b988-7c5ac8c9925d.png">


#### Step 6: Installing the make module using the below command

<img width="468" alt="image" src="https://user-images.githubusercontent.com/99624135/200434689-736bd2e6-aca1-4b3c-9e42-7e4025a8be8b.png">


#### Step 7: Installed the linux header of the current kernel to run the make command

<img width="468" alt="image" src="https://user-images.githubusercontent.com/99624135/200434838-ed480835-68e2-4c16-b0c1-2b44dc1a8180.png">


#### Step 8: Run the make command, use insmod to insert the module to the kernel, and display the features of the considered register.

<img width="468" alt="image" src="https://user-images.githubusercontent.com/99624135/200435184-2e9d1d10-827d-40ed-8754-2289678d3aef.png">
<img width="468" alt="image" src="https://user-images.githubusercontent.com/99624135/200435198-ddf46e18-edfd-4804-9e34-472624a2dd93.png">
<img width="468" alt="image" src="https://user-images.githubusercontent.com/99624135/200435205-d87aa64e-374e-4481-b214-e92a60aaf778.png">


#### Step 9: After adding the remaining structs and definitions, you'll see the below output

<img width="468" alt="image" src="https://user-images.githubusercontent.com/99624135/200435390-1bb3156b-47fc-48bb-a372-4463ecc5a87e.png">
<img width="468" alt="image" src="https://user-images.githubusercontent.com/99624135/200435404-7af6fa33-bc0a-4e6c-996e-1e2448c6a573.png">
<img width="468" alt="image" src="https://user-images.githubusercontent.com/99624135/200435413-a7a18a33-8a93-4565-a964-a9a0d74dfc7a.png">
<img width="468" alt="image" src="https://user-images.githubusercontent.com/99624135/200435426-e8839ff6-cae2-4fdc-91df-608251ddef2e.png">





