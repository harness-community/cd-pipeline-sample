# What is a pipeline?
A pipeline is a process that drives software development through a path of building, testing, and deploying code, also known as CD. By automating the process, the objective is to minimize human error and maintain a consistent process for how software is released. Tools that are included in the pipeline could include compiling code, unit tests, code analysis, security, and binaries creation. For containerized environments, this pipeline would also include packaging the code into a container image to be deployed across a hybrid cloud.

## How to use Pipline.yaml?
Change the code accordingly as shown here and paste the rest.
```
pipeline:
  name: <Name of the Pipeline>
  identifier: <Name of the Pipeline>
  projectIdentifier: <Name of the Project>
  orgIdentifier: default
```
