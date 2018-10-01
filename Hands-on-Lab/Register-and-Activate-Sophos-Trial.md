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





   

