# Harness Delegate

Our delegate serves two purposes. First, to provide a secure communication link between **Harness** and your **AKS Cluster**. Additionally, it allows Harness to delegate CI/CD tasks to your computer environment. Yeah, that’s why we named it the **delegate**. #NamingThingsIsHard. 

## Setup your Delegate in Azure Kubernetes Cluster
***

- Switch over to the **Harness UI** in another window. Navigate to your project under Project setup click on New Delegate

- Click on `New Delegate`

- Select **Kubernetes**, then click **Continue**.

- Enter “demo” in the Delegate **Name** field.

![Delegate Type ](/Images/delegate-type.png)


- Select **Small** for the Delegate Size.

- On the right side under Delegate Permissions select


![Delegate Size](/Images/delegate-size.png)


- Install Delegate with **cluster-wide read/write access**. Then click **Continue**.

- Click **Download YAML file**, then click **Continue**.


![Download YAML file](/Images/download-delegate.png)

- Switch Over to Azure Platform under kubernetes services select your resource and click on connect.

![Connect to Azure CLI](/Images/Azureconnect.PNG)

- Click on Open Cloud shell and follow the instructions given to set up your Azure cloud Shell.

- After successfull setup of Azure cloud shell click on the **Upload/Download files** option and select Upload.

![Azure CLI](/Images/AzureCLI.jpg)

- Upload the Yaml file which you have downloaded from the harness platform.

- After Successfull uploading of the file
Run the following command to apply the Harness Delegate to your Kubernetes Cluster
 
   ` kubectl apply -f harness-delegate.yml  `


- You should see output similar to this:

![Command Output in CLI](/Images/KubectlCommandoutput.PNG)


- Switch back to Harness platform,Harness will wait for your Delegate’s heartbeat, click **Done**

![Delegate Heart-Beat](/Images/delegate-heartbeat.png)




- The delegate should show **Connected** in a few minutes.

![Delegate succesfully connected](/Images/delegateConnected.PNG)









