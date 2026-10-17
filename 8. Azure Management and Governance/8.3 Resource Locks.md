Prevents resources from being accidentally deleted or changed.
Can be applied to resources, resource groups or even an entire subscription. Inherited from high to low. 
Managed from Azure Portal, PowerShell, Azure CLI or Azure Resource Manager Template.

To modify a locked resource, first remove the lock, then perform the activity you need to perform.

![](../Static/Pasted%20image%2020260930021651.png)

**Types of resource locks**

2 types. one that prevents deletion and one that prevents change and deletion

- Delete means authorized users can still read and modify a resource, but they can't delete the resource.
- ReadOnly means authorized users can read a resource, but they can't delete or update the resource. Applying this lock is similar to restricting all authorized users to the permissions granted by the Reader role.

