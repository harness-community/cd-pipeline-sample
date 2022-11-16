# What is a pipeline?
A pipeline is a process that drives software development through a path of building, testing, and deploying code, also known as CD. By automating the process, the objective is to minimize human error and maintain a consistent process for how software is released. Tools that are included in the pipeline could include compiling code, unit tests, code analysis, security, and binaries creation. For containerized environments, this pipeline would also include packaging the code into a container image to be deployed across a hybrid cloud.

# Import Pipeline
So, we are done with creating a project. Now, lets import a pipeline.

## Steps to import a  Pipeline
***

- Select the “**Create a pipeline**” button available at the top left corner of the page and then select “**Remote**”  

<img style="display:block;margin:48px auto;padding:1px;border:1px #eee;height:30%;width:70%;" src='../../Images/create-pipeline.png' />

- Enter the **name** as “testk8s”, and Add the **github connector** “testhelp” you created in the above step.  
- Under the **repository** section add “YAML-Onboarding-Harness” and select the **git branch** as `main`.  
- Now select **import**
  
## How to use Pipline.yaml present in /.harness folder?
Change the code accordingly as shown here and paste the rest.
```
pipeline:
  name: <Name of the Pipeline>
  identifier: <Name of the Pipeline>
  projectIdentifier: <Name of the Project>
  orgIdentifier: default
```

