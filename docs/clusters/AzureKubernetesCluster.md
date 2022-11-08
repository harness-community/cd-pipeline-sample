# Kubernetes Cluster


This guide demonstrates how to set up a Kubernetes cluster on AZURE.
## Setting up a Kubernetes Cluster 
***
### **Steps for creating Azure Kubernetes Cluster** 

### Create a Cluster

Step 1: Click on Kubernetes Services under Azure services after signing in.

![Azure Home Page](/Images/AzureHomePage.PNG)

Step 2: Click on Create a Kubernetes cluster under create the section.

![Azure Cluster Creation](/Images/CreateKubernetesClusterAzure.png)

Step 3:  On the Basics Tab, configure the following options to set up delegate:

#### Project Details:

- Select an Azure Subscription.

- Select or create an Azure Resource Group.

#### Cluster Details:

- Enter a Kubernetes cluster name.

- Select a Region for the AKS cluster.

- Select 99.5% for API server for a lower cost.

Step 4: Validate your resource by clicking on the **Review + create**  button.
After successful validation, click on **Create** to start building the cluster.

After a few minutes, your cluster will be deployed.

### Connect  to your cluster

When your cluster is ready click on connect.

Follow the instructions on the right to connect to your cluster.

Now you can set up your delegate using Azure Kubernetes cluster.

![image](/Images/ClusterConnectAzure.png)
