# AZURE-VIRTUAL-NETWORK-AND-SUBNETS

   
</head>
<body>
    <h1>How to Create Azure Virtual Network and Subnet </h1>
    <p>
        Follow these steps to add Azure Virtual Network and Subnet:
    </p>
    <ol>
        <li>
            <ul>
            </ul>
        </li>
        <li>
            <strong>Include Key Sections:</strong>
            <ul>
                <li><strong>Overview:</strong> Azure Virtual Network (VNet) is a fundamental building block for your private network in Azure. It enables Azure resources like virtual machines to securely communicate with each other, the internet, and on-premises networks. VNets are isolated from one another, providing security and segmentation. 
                   While Subnets are subdivisions within a VNet. They allow you to segment the virtual network into smaller, manageable sections. Each subnet can host resources and apply specific security or routing policies, helping organize and secure your network infrastructure. And the purpose of them in my project.</li>
                <li><strong>Prerequisites:</strong> List requirements such as an Azure account, Azure CLI, and necessary permissions.</li>
                <li><strong>Creation Steps:</strong> Provide step-by-step instructions to create a VNet and subnet. For example:
                    <pre>
az login
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
