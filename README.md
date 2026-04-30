# LogicApp-Fabric-Cost-Optimisation

Prereqs (do these once)

Enable System-assigned managed identity on the Logic App.
Give it:


Reader at the subscription scope(s) you query (so Resource Graph can return resources). A common pattern is Reader at subscription level for tag/resource discovery. [it-infrast....solutions]
Fabric capacity permissions to pause/resume (Microsoft lists required RBAC actions). [learn.microsoft.com]

