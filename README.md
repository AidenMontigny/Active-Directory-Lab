<h1> Active Directory Lab </h1>

<h2>Description</h2>
This project involved setting up and configuring an Active Directory environment to simulate enterprise-level access control and user management. A new domain, Montigny.com, was created and fully configured, including DNS verification. An organizational unit (OU) named CYB-515 was established, into which ten users were added using both command-line tools and PowerShell scripting. Five security groups were also created to structure user access. Default password policies were reviewed, then updated to enforce stronger security, and applied using gpupdate /force. This lab emphasized secure design principles such as least privilege, role-based access control, and policy enforcement—foundational elements in maintaining organizational security and infrastructure integrity.
<br />

<h2>Languages and Utilities Used</h2>

- <b> Powershell </b> 
- <b> Command Prompt </b>
- <b> Active Directory Users and Computers </b>
- <b> Group Policy Managment Console </b>
- <b> Windows Server Manager </b>
- <b> DNS Manager </b>

<h2>Environments Used </h2>

- <b> Windows Server 2019 </b>

<h2>Project walk-through:</h2>
<p align="left">
Documented the successful completion of the Active Directory installation selection process, <br/> confirming that all necessary components were properly configured for domain services <br/> deployment. <br/><br/>
  <img src="Screenshot 2025-04-17 202325.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
Configured the Root Domain Name as **Montigny.com**, establishing the foundational <br/> structure for the Active Directory domain environment. <br/><br/>
  <img src="Screenshot 2025-04-17 202331.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
  <p align="left">
Verified successful domain configuration through the login interface, which now reflects the <br/> domain name Montigny, confirming integration with the Active Directory environment. <br/><br/>
  <img src="Screenshot 2025-04-17 202340.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
  <p align="left">
Confirmed full server configuration by verifying that Server Manager components were <br/> populated correctly and that the `nslookup` command returned accurate DNS results, indicating <br/> successful Active Directory and DNS integration. <br/><br/>
  <img src="Screenshot 2025-04-17 202346.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
  <p align="left">
Created a new Organizational Unit (OU) titled **CYB-515** within Active Directory to logically <br/> group related users and resources, supporting structured administration and access control. <br/><br/>
  <img src="Screenshot 2025-04-17 202358.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
  <p align="left">
Created the first user account, 'Aiden Montigny', in Active Directory using command-line tools <br/> to demonstrate efficient user provisioning and adherence to administrative best practices. <br/><br/>
  <img src="Screenshot 2025-04-17 202404.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
  <p align="left">
Demonstrated the batch creation of nine additional user accounts via the command prompt, <br/> showcasing streamlined user provisioning within the organizational unit. <br/><br/>
  <img src="Screenshot 2025-04-17 202410.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
  <p align="left">
Confirmed the successful addition of all 10 user accounts within the designated organizational <br/> unit (OU), ensuring proper user management and directory structure. <br/><br/>
  <img src="Screenshot 2025-04-17 202415.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
  <p align="left">
Demonstrated the use of PowerShell commands to efficiently create five security groups within <br/> the organizational unit, supporting structured access control and group-based policy management. <br/><br/>
  <img src="Screenshot 2025-04-17 202421.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
  <p align="left">
Displayed the successful addition of the five security groups to the organizational unit, ensuring <br/> proper access control and group management within the Active Directory environment. <br/><br/>
  <img src="Screenshot 2025-04-17 202426.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
  <p align="left">
Displayed the default password policy settings within the Active Directory environment, <br/> outlining the initial configuration for password complexity and requirements. <br/><br/>
  <img src="Screenshot 2025-04-17 202435.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
  <p align="left">
 Displayed the updated password policy, which reflects the newly configured security requirements <br/> for user accounts in the domain. <br/><br/>
  <img src="Screenshot 2025-04-17 202441.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
  <p align="left">
Executed the ‘gpupdate /force’ command to enforce the application of the updated group policy, <br/> ensuring that the new settings take effect across the domain. <br/><br/>
  <img src="Screenshot 2025-04-17 202446.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>

<h2>Write Up</h2>

<p><u> Vulnerabilities and Risks of Access Control </u></p>
<p>Access control has many vulnerabilities and risks that pose a significant threat to an organization's infrastructure. Most vulnerabilities associated with AC are linked to authentication mechanisms or broad access permissions (HackerWhite, 2024). Without ensuring that there are robust AC measures, hackers have a platform for exploitation, which may lead to the access of confidential data, system alteration, financial losses, or much more. At the same time, if a company does not have any access control in place, it can be very detrimental. Access control aids in limiting the right to access critical data if not necessary. For example, if an organization did not have access control, an intern could potentially have access to the same amount of information as an executive employee, which could lead to detrimental circumstances for that organization.</p>

<p><u> Importance of Access Control Principles in Security </u></p>
<p>Access control principles are crucial for maintaining security by ensuring that only authorized users have access to specific data. For example, the principle of least privilege is key as it minimizes the potential damage of someone accessing data they are not intended to see. I believe that all companies should have a ‘need-to-know’ basis, which would aid in limiting the amount of access and knowledge employees have on the systems and data based on their role. Overall, AC is crucial for any company as it aids in ensuring its systems and data are safeguarded from misuse.</p>

<p><u> Common Security Failures in Workstations and Servers </u></p>
<p>Two of the most common security failures are inadequate patch management and access control. Inadequate patch management is when a system is not up to date with the latest security patches, leading to more vulnerabilities and security issues (Leyden, 2024). However, the issue sometimes will not be fixed by just updating the systems, as attackers can create their access before the update is put in place, leading to backdoor exploits. Access control issues all occur when permissions are not correctly configured, giving more access to users than they should have. These two issues can create significant issues for any organization and can lead to drastic financial losses.</p>

<p><u> Basic Security Implications of Modern Computing Environments </u></p>
<p>Modern computing environments, although beneficial, have some significant security issues. Some of these issues are data breaches, unauthorized access, and loss of control over data (Subramanian, 2018). Because modern computing environments are more complex, it has made ensuring security much harder and has led to some issues. However, with encryption, strong access control, and monitoring, these issues can be drastically reduced.</p>

<p><u> Developing Efficient System Solutions for Digital Assets </u></p>
<p>Developing efficient system solutions for digital assets requires security. Securing your digital assets typically involves encryption and MFA. As well, it is key to have a scalable system to ensure that it can meet the volume of assets being added. Overlapping balancing security and scalability for all digital assets is crucial, as it will create a robust framework for your system.</p>

<p><u> Hardware Components of Modern Computing </u></p>
<p>Modern computing relies on several key hardware components. These components include, but are not limited to, CPU, RAM, storage, GPU, PSU, and motherboard. All these components aid a computer in providing its intended functions.</p>

<p><u> Secure Design Principles for User Account Creation </u></p>
<p>To ensure that the user account creation is secure, a few things can be done. The first principle that should be applied is the least privilege. The least privilege ensures that the user only has access to information necessary for their job function. Secondly, applying authentication and authorization is crucial as it will aid in protecting against unauthorized access to accounts and data. Thirdly, monitoring user activities and ensuring that no suspicious activities are happening on any account or network is crucial to ensure security within the organization. Overall, applying different security measures for user accounts is crucial as it will aid the company's security posture and create a smaller attack surface for any malicious actors.</p>

<p><u> Comparing Virtualization in Windows and Linux Operating Systems </u></p>
<p>Both Windows and Linux OS have many pros; however, because they are so different, there could be more pros in using one over the other. For example, Windows is known for its VM managers such as Hyper-V and VMware, which are both used in most cyber professions (Henderson, 2022). However, they do come with a price and use a lot more resources than other Linux options. Linux has a VM manager named Docker, which is known for being lightweight and affordable. However, both Windows and Linux have great VM resources for any user; at the end of the day, it comes down to preference and what it is being used for.</p>

<p><u> References </u></p>
<p>Access control: Understanding & mitigating the risks in the Internal Network. HackerWhite. (n.d.). https://hackerwhite.com/vulnerability101/internal-network/access-control-vulnerability</p>
<p>Henderson, T. (2022, April 1). What is the difference between Linux and Windows?. Linode Guides & Tutorials. https://www.linode.com/docs/guides/linux-vs-windows/</p>
<p>Leyden, J. (2024, September 16). Patch Management: A dull pain that won’t go away. CSO Online. https://www.csoonline.com/article/3520881/patch-management-a-dull-it-pain-that-wont-go-away.html</p>
<p>Subramanian, N. (2018, July 19). Recent security challenges in cloud computing. Computers & Electrical Engineering. https://www.sciencedirect.com/science/article/abs/pii/S0045790617320724</p>



  
