Deployment and management service for Azure. It allows you to create, update and delete resources in Azure account.
User sends request. Azure Resource Manager receives the request. It authenticates and authorizes the request. It sends the request to the Azure Service which takes requested action. 

![](../Static/Pasted%20image%2020260930023429.png)

**Azure Resource Manager Benefits**

- Manage your infrastructure through declarative templates rather than scripts. A Resource Manager template is a JSON file that defines what you want to deploy to Azure.
- Deploy, manage, and monitor all the resources for your solution as a group, rather than handling these resources individually.
- Re-deploy your solution throughout the development life-cycle and have confidence your resources are deployed in a consistent state.
- Define the dependencies between resources, so they're deployed in the correct order.
- Apply access control to all services because RBAC is natively integrated into the management platform.
- Apply tags to resources to organize your subscription and support cost reporting.

**Infrastructure as Code**

This means managing infra through code and templates instead of manual configuration. This starts with Azure CLI and grows into repeatable environment deployments using Azure Resource Manager Templates and Bicep

**Azure Resource Manager Templates**

These describe desired Azure resources in declarative JSON. Azure validates template before deployment, then orchestrates resource creation in right order or in parallel. 
Templates can also call PowerShell or Bash scripts when needed.

**Benefits of using Azure Resource Manager Templates**

- **Declarative syntax**: Define what to deploy instead of writing step-by-step deployment commands.
- **Repeatable results**: Reuse the same template across environments for consistent outcomes.
- **Orchestration**: Azure Resource Manager handles dependency order and parallel deployment automatically.
- **Modularity**: Split templates into reusable components and nested templates.
- **Extensibility**: Add deployment scripts when additional setup actions are required.

**Bicep**

declarative language for deploying resources through ARM. Simpler and concise compared to JSON templates.

Benefits - 

- **Support for current Azure resources**: Bicep tracks Azure resource types and API versions.
- **Simple syntax**: Bicep is easier to read and write than equivalent JSON templates.
- **Repeatable deployments**: Bicep files are idempotent for consistent lifecycle deployments.
- **Built-in orchestration**: Azure Resource Manager handles dependencies and parallel deployment execution.
- **Modularity**: Reuse logic by organizing deployments into Bicep modules.