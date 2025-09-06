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

**Step 7: After loggin into the new domain with admin username and password, open the Windows PowerShell and run it as Administrator to create the new folder to store the PowerShell scripts in VM.**

<img width="1280" height="1024" alt="WinServer2022AD PowerShell new folder VM" src="https://github.com/user-attachments/assets/0d0a7c7f-015f-4511-bb45-49e497a06fcc" />

**Step 8: Import Active Directory Module in PowerShell to install Active Directory prior to creating organizational units.**

<img width="1280" height="1024" alt="WinServer2022AD PowerShell AD command" src="https://github.com/user-attachments/assets/ccab1be5-b78f-4b69-b7b4-ca5ef44f09bf" />

**Step 9: Create a Organizational Units (OUs) in PowerShell.**

<img width="1024" height="768" alt="WinServer2022AD NewOrganizationUnit" src="https://github.com/user-attachments/assets/53f54638-8e8c-48c7-8807-c151557c04e8" />
<img width="1024" height="768" alt="WinServer2022AD OrganizationUnit" src="https://github.com/user-attachments/assets/240745b1-53ea-450f-9e66-a1db7f740e8e" />
<img width="1024" height="768" alt="WinServer2022AD OrganizationUnit pt2" src="https://github.com/user-attachments/assets/8041fd42-8e5f-4c43-9698-e49cc2c25e52" />
<img width="1024" height="768" alt="WinServer2022 Ou in AD Users and Computers" src="https://github.com/user-attachments/assets/8a3fc532-d119-4dcc-a2f2-7d9a9078c005" />

**Step 10: Create a new ADUser with the command.**

<img width="1024" height="768" alt="WinServer2022 CreateADUser command" src="https://github.com/user-attachments/assets/00488f62-706f-45dd-b5fd-e743b57aa694" />

Create a new ADUser
<img width="1024" height="768" alt="WinServer2022 NewADUser" src="https://github.com/user-attachments/assets/11c9c4ef-9388-483b-bf3b-6ca9d5c8a0ab" />

Also Get-ADUser Identity cmdlet to retrieve information.
<img width="1024" height="768" alt="WinServer2022 ADUserIdentity" src="https://github.com/user-attachments/assets/af4d1c00-adf7-4d9e-af3b-a740e6fd87e4" />

<img width="1024" height="768" alt="WinServer2022 ADUserIdentity p2" src="https://github.com/user-attachments/assets/1773a1da-7654-4074-8d6f-c57870debe07" />

ADUser Filter cmdlet to filter out the search and retrieve desired user account.
<img width="1024" height="768" alt="WinServer2022ADUser Filter" src="https://github.com/user-attachments/assets/b28d0cbb-1583-4d7a-8521-590b49bf4b5b" />

<img width="1024" height="768" alt="WinServer2022 ADUser Filter with Pipeline" src="https://github.com/user-attachments/assets/683b02b0-9079-4149-b527-f76eade0a8a8" />

Set-ADUser email address and phone number plus change password.
<img width="1024" height="768" alt="WinServer2022 Set ADUser Email address" src="https://github.com/user-attachments/assets/a3da5e31-b072-432b-ba9b-508c2fab9f3d" />

<img width="1024" height="768" alt="WinServer2022 SetADUser Change Password" src="https://github.com/user-attachments/assets/d5a281d5-e172-46a3-b5f1-4d903cc7cd8e" />

<img width="1024" height="768" alt="WinServer2022 Set ADUser Office Phone Number" src="https://github.com/user-attachments/assets/6336c4c0-e144-404a-8570-39f982716837" />




