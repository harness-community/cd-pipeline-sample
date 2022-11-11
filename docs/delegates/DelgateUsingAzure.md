# Steps to Deploy Delegates on Azure Cloud
- After successful setup of Azure cloud shell click on the **Upload/Download files** option and select **Upload**.

![Azure CLI](/Images/AzureCLI.jpg)

- Upload the Yaml file which you have downloaded from the harness platform.

- After Successful uploading of the file
Run the following command to apply the Harness Delegate to your Kubernetes Cluster

```bash
kubectl apply -f harness-delegate.yml
```

- You should see output similar to this:

![Command Output in CLI](/Images/KubectlCommandoutput.PNG)

- Switch back to the Harness platform, Harness will wait for your Delegate’s heartbeat, click **Done**

![Delegate Heart-Beat](/Images/delegate-heartbeat.png)

- The delegate should show **Connected** in a few minutes.

![Delegate succesfully connected](/Images/delegateConnected.PNG)
