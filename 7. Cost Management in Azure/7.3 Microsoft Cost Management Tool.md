set of tools to help analyze, monitor and manage azure costs to avoid accidental provision of resources.

Cost Management provides the ability to check Resource costs, create alerts based on spend and create budgets that can be used to automate management of resources.

![](../Static/Pasted%20image%2020260930004646.png)

Cost analysis provides a visual for Azure costs. 
You can view total cost in diff ways, including by billing cycle, region, resource etc.
You can view aggregated costs by subscription, resource group or service to identify spending trends.

**Cost Alerts**

Provides a single location to check all different alert types that show up. 3 types are - 
1. Budget alerts
2. Credit Alerts
3. Department spending quota alerts

**Budget Alerts**

Notify when spending reaches a defined threshold.
Can create budgets in Azure portal or in Azure Consumption API
In Azure portal, budgets are defined by costs, in Azure Consumption API, you can define budgets by consumption usage. 
When an alert is generated, it appears in cost alerts and an alert email is also sent to people in alert recipient list.

**Credit Alerts**

Notifies when your Azure Prepayment is consumed. Azure prepayment is for organizations with Enterprise Agreements (EAs). Credit alerts are generated automatically at 90% and 100% of your Azure Credit Balance. 

**Department Spending Quota Alerts**

These are specific to EAs customers. Notify when your department spending reaches a fixed threshold of the quota. 
Spending quotas are defined in Azure Portal. 

**Budgets**

Spending limit for Azure. Set budgets based on subscription, resource groups, service type or other criteria. 
When you set a budget, you also set a budget alert.
You can also configure budgets to trigger automation that suspends or modifies resources when a spending threshold is reached. 
For Example, automate shutdown of non production resources when a budget is reached.