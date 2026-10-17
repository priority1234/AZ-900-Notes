Azure provides multiple tools for managing your environment - 
1. Azure Portal
2. Azure PowerShell
3. Azure Command Line Interface (CLI)

Can also use copilot to accelerate common operations tasks like exploring services, understanding configuration options etc.

![](../Static/Pasted%20image%2020260930022217.png)

**AI Assisted operations with Copilot in Azure**

Copilot in Azure is an AI assistant experience that can help administrators work faster by providing contextual guidance in natural language. Depending on your environment, some Copilot workflows can be agent-like, where the assistant helps coordinate multi-step tasks.

**Azure Portal**

Web-based unified console. You can manage Azure subscription using a GUI. You can - 
- Build, manage, and monitor everything from simple web apps to complex cloud deployments
- Create custom dashboards for an organized view of resources
- Configure accessibility options for an optimal experience

**Azure Cloud Shell**

Browser based shell tool, that allows you to create, configure and manage Azure resources using shell. 
Supports Azure PowerShell and Azure CLI which is a Bash shell

some features are - 
- It is a browser-based shell experience, with no local installation or configuration required.
- It is authenticated to your Azure credentials, so when you log in it inherently knows who you are and what permissions you have.
- You choose the shell you’re most familiar with; Azure Cloud Shell supports both Azure PowerShell and the Azure CLI (which uses Bash).

**Azure PowerShell**

Used to run commands known as command-lets (cmdlets). These call Azure REST API to perform management tasks in Azure. 
Cmdlets can be run independently to handle one-off changes or they can be combined to help orchestrate complex actions like - 

- The routine setup, teardown, and maintenance of a single resource or multiple connected resources.
- The deployment of an entire infrastructure, which might contain dozens or hundreds of resources, from imperative code.

You can also install and configure Azure PowerShell on Windows, Linux and MacOS

**Azure CLI**

Equivalent to Azure PowerShell with difference being the syntax of commands. It uses Bash commands.