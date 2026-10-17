Hosting Service for DNS Domains that provides name resolution by using Azure infra. 

**Benefits** -

- Reliability and performance
- Security
- Ease of use
- Customizable virtual networks
- Alias records

**Reliability and Performance** -

DNS domains in Azure DNS are hosted on Azure's global network of DNS name servers. 
It uses anycast networking, so the closest available DNS server answers each DNS query

**Security** -

Based on Azure Resource Manager which provides features like Azure RBAC, activity logs and resource locks to protect DNS resources and records

**Ease of Use** -

Can manage DNS records for Azure services and also provide DNS for external resources.
Integrated into the Azure portal and uses the same credentials, support contract and billing as other Azure services.
Allows you to manage your domains and records with Azure portal, PowerShell cmdlets and Azure CLI. 

It also supports private DNS domains, so you can use your own custom domain names in your private virtual networks instead of Azure provided names.

**Alias Records** -

supports alias record sets. You can use alias record set to refer to an Azure resource. if the IP address of resource changes, the alias also updates itself to point at the new IP. 