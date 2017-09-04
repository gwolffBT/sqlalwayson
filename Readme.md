# Create base Azure infrastructure resources for SQL Server AlwaysOn Availability Group (AOAG) in an _existing_ Azure VNet and Active Directory domain.

This template creates the following resources:
+	One internal load balancer (ILB) to be used for AOAG listener
+	Three VMs in a Windows Server Failover Cluster (WSFC)
	+	Two VMs run SQL Server Enterprise
	+	The third VM is the File Share Witness for the cluster
+	One Managed Availability Set for the SQL and Witness VMs
+	All VMs are provisioned using Premium Managed Disks

## Deploying

You can deploy these samples directly through the Azure Portal by clicking the button below or by using the deploy.ps1 script supplied in the root of this repo.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Frobotechredmond%2F301-sql-alwayson-ag-cluster-base%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

