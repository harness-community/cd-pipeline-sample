# Kubernetes Cluster

Here, we will discuss how you can set up a K8's cluster with GCP

## Setting up a Kubernetes Cluster 
***
### **Steps for Google Cloud Provider** 

- [Create a project in GCP](https://developers.google.com/workspace/guides/create-project), click on left panel and select the **Kubernetes Engine**.
- Click on Clusters and you should see the existing set of clusters created under this project.
- Click on **+ Create** on the top and start with the GKE Standard. Click **Configure**.
- Name the cluster, select the location(zone).
- Select the **node configuration** and provision the cluster.

It takes a few minutes for the cluster to be ready for use.  
Once you cluster show the Green tick with other config details, it is all set to be used.
You can connect it from this [GCP console](https://cloud.google.com/binary-authorization/docs/getting-started-console) by selecting your cluster and then click on Connect on the top. It will open a console and you are ready to run Kubernetes commands and play around the cluster.


### **Creating the Namespace**
**Namespaces** are one of those things that are so simple, they’re hard to understand. And since they deal with naming things… well… they can be hard. For our purposes, a namespace is a way to subdivide your cluster. They’re super useful for isolating different services that run in the same cluster. We need you to create a namespace called ‘demo’. 

### Create the namespace with `kubectl`:
```console 

$ kubectl create namespace demo
namespace/demo created

```
