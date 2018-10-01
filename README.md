# Sophos-on-Azure

Sophos XG Firewall is a next-generation firewall you can select and launch from within the Microsoft Azure Marketplace. XG Firewall deploys as an all-in-one solution that combines advanced networking, protections such as Intrusion Prevention (IPS), and web application firewalling (WAF), as well as user and application controls. XG Firewall is designed to help you protect your Azure-based workloads against advanced threats.


<!-- TOC -->
1. [AEC Registeration experience](#aec-registeration-experience)  
2. [Register and Activate Sophos Trial](#register-and-activate-sophos-trial)    
3. [Verify IIS Website Working ](#verify-iis-website-working)    
4. [Remove Public IP from Windows VM](#remove-public-ip-from-windows-vm)      
5. [Configure Web Application Firewall in Sophos and Public the IIS Website via XG](#configure-web-application-firewall-in-sophos-and-public-the-iis-Website-via-xg)      




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

4. After the lab is deployed, the lab details will be displayed as given below:  
<img src="/images/odl details.png"/>  

# Pre-deployed envrionment  

To login in to the pre-deployed sophos environment proceed as follows:  

1. From the **ODL details** page copy the username and password.  
<img src="/images/username and password odl.png"/>    


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


# Verify IIS Website Working

To verify whether the already deployed IIS Website is working, proceed as follows:  

1. Login into [Azure](https://portal.azure.com/) with the provided credentials.  
2. Go to the resource group that is being used in the lab.  

3. In the **Overview** section, select **iis-vm**.  
<img src="/images/select iis vm.png"/>  

4. In the **Overview** blade of the **iis-vm**, copy the **DNS name** of the VM.  
<img src="/images/copy dns of iis vm.png"/>    

5. **Paste** the copied **DNS name** of the iis-vm in any browser. If you get the below webpage you can confirm that the Website is working properly.  
<img src="/images/webserver working properly.png"/>  


# Remove Public IP from Windows VM  

1. Login into [Azure](https://portal.azure.com/) with the provided credentials.  
2. Go to the resource group that is being used in the lab.  

3. In the **Overview** section, select **iis-pip**.  
<img src="/images/select iis pip.png"/>  

4. In the **Overview** blade of the **iis-pip**, **click** on **Dissociate**.  
<img src="/images/dissociate pip.png"/>  

5. On clicking Dissociate, you will get the following pop-up. **Click** on **Yes** to continue.  
<img src="/images/dissociate yes.png"/>  

6. Navigate to the **Overview** blade of the Resource group and select **iis-vm**.  
<img src="/images/select iis vm.png"/>  

7. In the **Overview** blade of the **iis-vm** you can see that the **Public IP address** and  **DNS name** have disappeared.  
<img src="/images/pip gone.png"/>  


# Configure Web Application Firewall in Sophos and Public the IIS Website via XG  

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

7.  In the Sophos XG Firewall Dashboard, under the **Protect** section, **Select** **Web Server**.  
<img src="/images/select web server.png"/>  

8. Click on **Add** to enter the details of the Web Server.  
<img src="/images/add web browser.png"/>    

9. Enter the **Name** to be given to the Webserver. For **Host**, click on the drop-down box corresponding to the Host.  
<img src="/images/web server details image 1.png"/>  

10. Click on **Create new** and then on **IP Host**.    
<img src="/images/create new.png"/>  

11. Enter the follwing details:  
    * Name: **Enter the name for the webserver.**  
    * IP Version: **IPv4**  
    * Type: **IP**  
    * IP Address: **Enter the Private IP address of the iis-vm**
    
    After entering the details, click on **Save**.  
<img src="/images/Add IP host.png"/>  

12. Keep the rest of the values as default and click on **Save**. Now the Web Server will be added successfully.   
<img src="/images/add web server image 2.png"/>  

13. Now in the Sophos XG Firewall Dashboard, Under the **PROTECT** section, click on **Firewall**. Now click on **Add Firewall Rule**.  
<img src="/images/add firewall click.png"/>  

14. Click on **Business Application Rule**.  
<img src="/images/business applciation rule select.png"/>  



