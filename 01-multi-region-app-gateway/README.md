# Multi-Region Web App Deployment Using Azure VM, Application Gateway & Traffic Manager

This project demonstrates how to host a multi-region application with:

- **Azure Virtual Machines (VM1 and VM2)**: to host the Upload and Home pages
- **Azure Blob Storage (Static Website Hosting)**: to host custom error pages like 403 and 502
- **Azure Application Gateway**: with path-based routing to direct `/` to home and `/upload` to upload page
- **Azure Traffic Manager**: to load balance traffic between Central US and West US regions
- **VNet Peering**: to connect VNets across regions

Key deployment steps include:
- Clone GitHub repo to VM1 and VM2
- Run `vm1.sh` on VM1 to deploy the Upload page
- Run `vm2.sh` on VM2 to deploy the Home page
- Configure Azure Application Gateway to use error.html from Blob Storage
- Configure Traffic Manager to route to both Application Gateways
