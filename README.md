# Sophos-on-Azure

Sophos XG Firewall is a next-generation firewall you can select and launch from within the Microsoft Azure Marketplace. XG Firewall deploys as an all-in-one solution that combines advanced networking, protections such as Intrusion Prevention (IPS), and web application firewalling (WAF), as well as user and application controls. XG Firewall is designed to help you protect your Azure-based workloads against advanced threats.


<!-- TOC -->

1. [Register and Activate Sophos Trial](/Hands-on-Lab/Register-and-Activate-Sophos-Trial.md)  
2. [Verify IIS Website Working ](/Hands-on-Lab/Verify-IIS-Website-Working.md)  
3. [Remove Public IP from Windows VM](/Hands-on-Lab/Remove-Public-IP-from-Windows-VM.md)    
4. [Configure Web Application Firewall in Sophos and Public the IIS Website via XG](/Hands-on-Lab/Configure-Web-Application-Firewall-in-Sophos-and-Public-the-IIS-Website-via-XG.md)    




<!-- /TOC -->

# AEC Registeration Experience  

1. Navigate to the URL provided to sign-up for the lab.  

2. Enter the following details:  
   * **First Name**  
   * **Last Name**  
   * **Work email**  
   * **Organization**  
   * **Country**  
   
   After entering the details click on **SUBMIT**.  
   
<img src="/images/AEC registeration.png"/>  

3. After entering the details, **click** on the **LAUNCH LAB** button to proceed further.      

<img src="/images/launch lab button.png"/>  


# Register and Activate Sophos Trial

## Registering for Sophos Trial

To activate a trial version of Sophos XG Firewall proceed as follows:  

1.  Follow this [link](https://secure2.sophos.com/en-us/products/next-gen-firewall/free-trial.aspx) to register for the trial license of Sophos XG Firewall.  

2.  Enter the following details in the signup page  
    * **First Name**    
    * **Last Name**  
    * **Business Email**  
    
    After entering the above details click on **Next**.   

<img src="/images/sophos trial signup image 1.png"/>  

3. On clicking Next, you will be redirected to the next page to enter further details.  
   * **Job Role**  
   * **Phone number**  
   * **Company**  
   * **Industry**  
   * **Company Size**  
   * **Country**  
   * **State/Province**  
   * **Check the terms and conditions statement**.  
   
   After filling the above details click on **Submit**.  
   <img src="/images/sophos trial signup image 2.png"/>  
   
4. You wil now receive a mail with the serial number for your trial license.  
   
   <img src="/images/sophos seiral number mail.png"/>    

## Activating Sophos Trial  

To activate the Sophos trial version proceed as follows:  

1. Login to Azure by using the provided credentials. To login to azure go to [portal.azure.com](https://portal.azure.com/)  

2. After logging in, **Click** on **Resource Groups** and then select the resource group as shown below.  
<img src="/images/selecting rg.png"/>  

3. In the **Overview** section, select the **sophos-vm**.  
<img src="/images/selecting sophos vm.png"/>  

4. In the **Overview** blade of the **sophos-vm**, **copy** the **DNS name** of the VM.  
<img src="/images/copy dns of sophus vm.png"/>  

5. Paste the following URL in any browser *https://DNSname:4444* (Replace the 'DNSname' with the DNS name of the Sophos VM) to go to the Web UI of the Sophos XG Firewall.  

6. Enter the following details.  
   * Username: **admin**  
   * Password: **labPassword1!**  
   
   After entering the details click on **Login**. 
<img src="/images/sophos login.png"/>  

7. To register the trial license, choose **I have an existing serial number** and enter the **Serial Number** you recieved via email. After entering the Serial Number **Click** on **Continue**.    
<img src="/images/serial number entering.png"/>  

8. Now you will be prompted to create a **Sophos ID**. To create a Sophos ID click on **Create Sophos ID**.  
<img src="/images/sophos id creation.png"/>  

9. You will be redirected to a page to create the **Sophos ID**. Enter the following details:  
   * **First Name.**  
   * **Last Name**  
   * **Email Address**  
   
   After entering the details click on **Register**.  
   <img src="/images/sophos id details.png"/>  
   
10. You will now receive a mail with a link to confirm the Sophos ID registeration. Click on the link to proceed.  
<img src="/images/sophos id confirmation.png"/>  

11. On clicking the link you will be redirected to a page where you will be promoted to set a new **password** for your Sophos ID. After entering the new password **click** on **Save Password**.    
<img src="/images/sophos id password set.png"/>  
   

12. Now navigate back to the **Sophos Device Management** page to sign in using the newly created **Sophos ID**.  
<img src="/images/sophos device mgmt page.png"/>  

13. You will now be prompted to enter the **email address** which was used to create the **Sophos ID** and the **password** to **Sign In**.  
<img src="/images/signing in using sophos id.png"/>    

14. Now you will receive a message to register the device in which you have installed the Sophos XG Firewall. The device will be given a unique ID as shown below. **Click** on **Continue** to proceed.  
<img src="/images/sophos device registeration.png"/>  

15. Enter the **Company** Name and **Country** and **Click** on **Continue**.  
<img src="/images/company name and country.png"/>    

16. The **Device details** will be displayed. **Click** on **Confirm Registeration** to proceed.  
<img src="/images/deve details confirmation.png"/>  

17. **Click** on the **Initiate License Synchronization** button to **Continue**.  
<img src="/images/initate license sync.png"/>  

18. The Basic Setup is now completed. **Click** on **Continue** to Proceed further.  
<img src="/images/basic setup complete.png"/>  

