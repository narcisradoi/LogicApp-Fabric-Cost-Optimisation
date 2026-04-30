# LogicApp-Fabric-Cost-Optimisation

Prereqs (do these once)

**Enable System-assigned managed identity on the Logic App.**
Give it:
Reader at the subscription scope(s) you query (so Resource Graph can return resources). A common pattern is Reader at subscription level for tag/resource discovery.
Fabric capacity permissions to pause/resume (Microsoft lists required RBAC actions).

**The identity must have these permissions on the Fabric capacity resource:**
Microsoft.Fabric/capacities/read
Microsoft.Fabric/capacities/write
Microsoft.Fabric/capacities/suspend/action
Microsoft.Fabric/capacities/resume/action

**Tags to use**
Example: tag your Fabric capacities like:
Key: AutoPause
Value: true

(You’ll set these in the workflow parameters below.)
