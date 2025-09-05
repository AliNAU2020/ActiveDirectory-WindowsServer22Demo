# ActiveDirectory-WindowsServer22Demo
Demo setup of an Active Directory using PowerShell on a Windows Server 2022 VM in Oracle VirtualBox.

This project will provide a fully automated demo environment for setting up Active Directory on a Windows Server 2022 virtual machine using Windows PowerShell scripts inside the Oracle VirtualBox. Ideal for learning, testing, and showcasing AD setup and management.

Here are the steps I did to build Active Directory Demo HomeLab.

**Step 1: Create a virtual machine by clicking on "New" in VirtualBox, naming it "WinServer2022AD" and selecting "Windows 10 (64 bit)" as boot media.**

<img width="2355" height="1257" alt="Creating a New Virtual Machine (AD Demo)" src="https://github.com/user-attachments/assets/5cb17bb4-7e34-4d48-94fd-9d3d6b8bd572" />

<img width="2353" height="1239" alt="Creating a New Virtual Machine (AD Demo) pt2" src="https://github.com/user-attachments/assets/a8cad372-5fa6-49dd-a378-fb9a937f3646" />

<img width="2361" height="1255" alt="Creating a New Virtual Machine (AD Demo) pt3" src="https://github.com/user-attachments/assets/21548ac2-cb60-40b9-a802-cbea94fa2b78" />

**Step 2: Once the configuration virtual machine is done, the virtual machine will start and the operating system setup will occur.**

<img width="1024" height="768" alt="Setup WinServer22 AD" src="https://github.com/user-attachments/assets/6c5d5137-8cd6-4f9e-a41e-26433757c789" />

**Step 3: Once the operating system is installed in the VM, the language is selected which is English, then next page, it asks what operating system you want to install on VM. So I clicked Windows Server 2022 Desktop Edition.**

<img width="1024" height="768" alt="Setup WinServer22 OS AD" src="https://github.com/user-attachments/assets/eb1d7993-103f-4504-aa7d-d7d415c1a154" />

**Step 4: The VM will startup and the the domain login page displays. Enter the password on domain account and it takes you to Server Manager.**

<img width="1024" height="768" alt="WinServer22 Admin Login Page" src="https://github.com/user-attachments/assets/196ba808-440b-42e2-b17d-3a6f3bb8da04" />

<img width="1024" height="768" alt="WinServer2022AD Server Manager" src="https://github.com/user-attachments/assets/f6af5061-ba1f-4771-b60c-616694817cf7" />

**Step 5: Name the domain and Install Active Directory Domain Service to create the domain.**

<img width="1024" height="768" alt="WinServer2022AD Active Directory Installation" src="https://github.com/user-attachments/assets/75fb9d27-ae12-456b-b784-f810421550fc" />
<img width="1024" height="768" alt="WinServer2022AD Domain Name" src="https://github.com/user-attachments/assets/3891a469-1891-47d5-839b-0c7fae757f4f" />

**Step 6: Once the domain is created, the VM is rebooted and sign in with the domain name and password used after VM creation.**

<img width="1280" height="1024" alt="WinServer2022AD Domain Account Login Page" src="https://github.com/user-attachments/assets/37cd07c4-2885-44c6-aca2-502896ab63b7" />



