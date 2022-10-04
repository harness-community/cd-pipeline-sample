# Harness Delegate

Our delegate serves two purposes. First, to provide a secure communication link between **Harness** and your **GKE Cluster**. Additionally, it allows Harness to delegate CI/CD tasks to your compute environment. Yeah, it’s why we named it the **delegate**. #NamingThingsIsHard. 

So, now you need to create a delegate to continue. And by create, I mean you need to install the delegate in your compute environment. If you’re familiar with the abbreviation k8s, then by all means - install the delegate. 

/ image to be

If you’re a bit earlier on the learning curve - say you know in theory what k8s is but, have never used it before that’s ok. We’ve got your back, and we all started out knowing less than you do now. Follow below, and we’ll walk through all the steps needed to set up a delegate.   



## Setup your Delegate 
***

- Switch over to the **Harness UI** in another window. Navigate to your project and when you see the ‘There are no Delegates in your project’ screen like the screenshot above then:

- Select **Kubernetes**, then click **Continue**.

- Enter “demo” in the Delegate **Name** field.

/ image to be

- Select **Small** for the Delegate Size.

- On the right side under Delegate Permissions select

/ image to be

- Install Delegate with **cluster-wide read/write access**. Then click **Continue**.

- Click **Download YAML file**, then click **Continue**.

/ img to be

- Harness will wait for your Delegate’s heartbeat, click **Done**

/ img to be

- Open a **terminal** in the directory where you downloaded the **YAML file**. Use `kubectl` to apply the configuration.

- You should see output similar to this:   
```console
$ kubectl apply -f harness-delegate.yml
namespace/harness-delegate-ng created
clusterrolebinding.rbac.authorization.k8s.io/harness-delegate-ng-cluster-admin created
secret/demo-proxy created
statefulset.apps/demo created
service/delegate-service created
```

- The delegate should show **Connected** in a few minutes.

/img to be









