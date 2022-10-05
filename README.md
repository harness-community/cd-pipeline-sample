# Continuous Delivery Pipeline Sample

![Cover Image CD Pipeline](Images/harness_cover_image.png)

This sample repository shows how to use the [Harness Continuous Delivery Pipeline](https://harness.io/products/continuous-delivery) to deploy a nginx image to Google Kubernetes Engine using YAML based pipeline creation.



## Getting Started

```mermaid
graph LR

PreFlightChecklist --> Cluster --> Delegate --> Secrets --> Connectors --> Project --> Pipeline --> PipelineExecution

```

![CD Pipeline](Images/harness-cd-architecture.png)
## Layout

| Docs | Description | Link |
| --- | --- | --- |
| PreFlight Checklist | A checklist for all the pre-requisites | [Click Here](docs/PreFlightChecklist.md) |
| Cluster | Steps to set up GKE | [Click Here](docs/clusters) 
| Delegate | Steps to set up the Harness Delegate  | [Click Here](docs/delegates) |
| Secrets | Learn about Secrets and steps to set them up | [Click Here](docs/secrets) |
| Connectors | Steps the to set up Docker and GitHub Connectors  | [Click Here](docs/connectors) |


## Contributors

<a href="https://github.com/harness-community/cd-pipeline-sample/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=harness-community/cd-pipeline-sample" />
</a>




## License

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

