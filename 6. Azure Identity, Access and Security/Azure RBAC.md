Principle of least privilege - Only grant access to the minimum level needed to complete a task.

Azure provides built in roles that describe common access roles for cloud resources. 
Can also define custom roles.
When an individual or groups are assigned a role, they receive all associated permissions

**RBAC for Resources**

![[Pasted image 20260929234513.png]]

RBAC is applied to a scope. a scope can be a group, subscription, resource group or individual resource.

Azure RBAC is hierarchical i.e. when you grant access at parent scope, all child scopes inherit that access.
- When you assign the Owner role to a user at the management group scope, that user can manage everything in all subscriptions within the management group.
- When you assign the Reader role to a group at the subscription scope, the members of that group can view every resource group and resource within the subscription.

