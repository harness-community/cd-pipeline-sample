#  Get Started with Azure Kubernetes.

# Harness Delegate

Our delegate serves two purposes. First, to provide a secure communication link between *Harness* and your *AKS Cluster. Additionally, it allows Harness to delegate CI/CD tasks to your computer environment. Yeah, that’s why we named it the **delegate*.

## Setup your Delegate in Azure Kubernetes Cluster
***

- Switch over to the *Harness UI* in another window. Navigate to your project under Project setup click on *New Delegate*

- Click on `New Delegate`

- Select *Kubernetes, then click **Continue*.

- Enter “demo” in the Delegate *Name* field.

![Delegate Type ](/Images/delegate-kubernetes-type.png)


- Select *Small* for the Delegate Size.

- On the right side under Delegate Permissions select *Install Delegate with cluster-wide read/write access.Then click **Continue*.


![Delegate Size](/Images/delegate-small-size.png)


- Click *Download YAML file, then click **Continue*.


![Download YAML file](/Images/download-delegate-yaml.png)

- Switch Over to Azure Platform under *Kubernetes services* select your resource and click on *Connect*.

![Connect to Azure CLI](/Images/Azureconnect.PNG)

- Click on *Open Cloud shell* and follow the instructions given to set up your Azure cloud Shell.

