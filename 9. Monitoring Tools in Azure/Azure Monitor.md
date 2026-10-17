Platform for collecting, analyzing and acting on data from Azure resources and applications. 
It works with Azure, on-prem and multicloud environments.

![[Pasted image 20260930024649.png]]

It gathers logs and metrics from your apps, OS and network layers. Stores it centrally and makes it available through dashboards, queries and alerts.

**Azure Log Analytics**

This is the tool where you write and run Queries against the data Azure Monitor collects. 
You can do filtering or run advanced analytics to visualize trends over time.

**Azure Monitor Alerts**

Alerts notify you when Azure Monitor detects a condition you defined has been met. 
You create a rule an an action group that controls who gets notified and what happens next.
Alerts can be metric based or log-based. Example - a metric alert can send you an email when a VM's CPU stays above 80%, while a log alert can watch for a specific error pattern across multiple resources. Action groups are reusable across Azure Monitor, Service Health, and Azure Advisor.


**Application Insights**

This is an Azure Monitor feature that monitors the performance and usage of your web applications, whether they run in Azure, on-prem or in another cloud.

You can set up Application insights by adding an SDK to your app code. 

Application Insights can monitor:

- Request rates, response times, and failure rates
- Dependency calls and their performance
- Page load times, user counts, and session trends
- Server performance counters such as CPU, memory, and network usage

You can also set up availability tests that send synthetic requests to your application so you know it's responding, even during low-traffic periods.

