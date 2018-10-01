# Configure WAF(Web Application Firewall) in Sophos and Public the IIS Website via XG  

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

10. Click on **Create new**.  
<img src="/images/create new.png"/>  

