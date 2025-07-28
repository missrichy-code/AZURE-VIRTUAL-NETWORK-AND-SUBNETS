# AZURE-VIRTUAL-NETWORK-AND-SUBNETS

   
</head>
<body>
    <h1>How to Create Azure Virtual Network and Subnet </h1>
    </p>
    <ol>
               <l>   Aim Of Project: To Setup A Secure Cloud Infracstructure For A Financial Institute
            <ul>
            </ul>
            <ul>
                <li><strong>Overview:</strong> Azure Virtual Network (VNet) is a fundamental building block for your private network in Azure. It enables Azure resources like virtual machines to securely communicate with each other, the internet, and on-premises networks. VNets are isolated from one another, providing security and segmentation. 
                   While Subnets are subdivisions within a VNet. They allow you to segment the virtual network into smaller, manageable sections. Each subnet can host resources and apply specific security or routing policies, helping organize and secure your network infrastructure. And the purpose of them in my project is to create a server for a required organization.</li>
                <li><strong>Prerequisites:</strong> Azure account, Azure CLI, MING, AZURE FIREWALL, DDOS NETWORK PROTECTION.</li>
                <li><strong>Creation Steps:</strong> step-by-step instructions to create a VNet and subnet. 
                    <pre>
Login to your portal
Go to Cost Management+Billing
Click on Billing
Select Benefits(preview)
Under the preview there's always a free service                        
Go to Virtual Network and Click Create  
Create a new Resource group 
<img width="722" height="358" alt="1Screenshot 2025-07-25 091205" src="https://github.com/user-attachments/assets/7ae85ff9-d668-497c-80b5-54af87b59764" />
Goto instance detail and give it a VM name 
Select your desired region
Click on next (Security)
Enable Azure Firewall
<img width="778" height="386" alt="4Screenshot 2025-07-25 103345" src="https://github.com/user-attachments/assets/dd14a3b9-d3f2-4c3b-8a15-d5a418040159" />
Enable DDOS Network Protection
<img width="827" height="392" alt="5Screenshot 2025-07-25 103444" src="https://github.com/user-attachments/assets/4c1e65ea-a9df-43a2-b2e5-95782fd2566b" />
NB: Azure Firewall and DDOS Network Protection are not free servives
Then Review and Create 
<img width="938" height="391" alt="6Screenshot 2025-07-25 105002" src="https://github.com/user-attachments/assets/f4657b7f-2923-4194-8cef-d5210805c220" />
After deployment is successful, Go to your Resource
Go to Settings (Click on Subnet)
Leave name at default
<img width="950" height="393" alt="8Screenshot 2025-07-25 105253" src="https://github.com/user-attachments/assets/277c05a9-6b7b-4ecd-bd48-a9cf9a8fb0e0" />
<img width="949" height="434" alt="9Screenshot 2025-07-25 105502" src="https://github.com/user-attachments/assets/153c8918-0ce9-4437-a1b1-1c0d493ea040" />
You can also get Microsoft Defender for cloud is Settings too
To Deploy Windows/Linux VMs using Azure B1s 
Go to cost Management+Billing
Click on Billing, Select Benefits(preview)
<img width="890" height="424" alt="10Screenshot 2025-07-25 105810" src="https://github.com/user-attachments/assets/4f1bde23-3376-4a1d-aabc-8a7bd46ae023" />
Select View all free services
Select Linux Virtual Machine (750hrs) then Create
<img width="955" height="391" alt="11Screenshot 2025-07-25 105913" src="https://github.com/user-attachments/assets/0380cba4-43f7-4358-8245-cc3d3f2f8266" />
Select your resource group
Input the VM name and Region
Image- (Ubuntu Server 22.04 LTS 64 Gen 2)
<img width="929" height="398" alt="Screenshot 2025-07-25 110055" src="https://github.com/user-attachments/assets/de2c8fa0-1696-44bc-8fc6-07bc094ceff3" />
Select password in Authentication type 
Username- Azureuser
Then out a strong password
Select inbound ports (HTTP(80), SSH(22))
<img width="841" height="402" alt="Screenshot 2025-07-25 110823" src="https://github.com/user-attachments/assets/6767de63-f3db-42df-b4e2-e0e773b05e87" />
Review and Create
<img width="837" height="392" alt="Screenshot 2025-07-25 111014" src="https://github.com/user-attachments/assets/beec3cbd-8344-438a-89c7-0857e1aa3717" />
Then go to your MING 
Type ssh azureuser@copy and paste public IP address
Then Enter
Put your password 
<img width="816" height="425" alt="Screenshot 2025-07-25 111945" src="https://github.com/user-attachments/assets/aedefb15-e2b1-4d6b-a78d-116ff8633418" />
With this you've created a secure server for the Financial Institution

az group create --name &lt;resource-group&gt; --location &lt;location&gt;
az network vnet create --resource-group &lt;resource-group&gt; --name &lt;vnet-name&gt; --address-prefix &lt;address-prefix&gt;
az network vnet subnet create --resource-group &lt;resource-group&gt; --vnet-name &lt;vnet-name&gt; --name &lt;subnet-name&gt; --address-prefix &lt;subnet-prefix&gt;
                    </pre>
                </li>
                <li><strong>Configuration:</strong> Explain how to configure network security groups, route tables, and other settings.</li>
                <li><strong>Troubleshooting:</strong> Add common issues and solutions.</li>
                <li><strong>References:</strong> Link to official Azure documentation.</li>
            </ul>
        </li>
        <li>
            <strong>Commit and Push:</strong>
            <ul>
                <li>Commit your documentation file and push it to your GitHub repository.</li>
            </ul>
        </li>
        <li>
            <strong>Keep Documentation Updated:</strong>
            <ul>
                <li>Update the documentation as your network setup or configuration changes.</li>
            </ul>
        </li>
    </ol>
    <p>
        For more details, see the <a href="https://learn.microsoft.com/en-us/azure/virtual-network/">Azure Virtual Network Documentation</a>.
    </p>
</body>
</html>
