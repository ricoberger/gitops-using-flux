# GitOps using Flux: How we manage Kubernetes clusters at Staffbase

Repository for my talk at the **Kubernetes and Cloud Native Meetup Dresden** about GitOps using Flux on the 30. January 2020.

- Presentation: [GitOps using Flux: How we manage Kubernetes clusters at Staffbase](./assets/gitops-using-flux.pdf)
- Twitter: [@rico_berger](https://twitter.com/rico_berger)

## What is GitOps?

*"GitOps is a way to do Kubernetes cluster management and application delivery. It works by using Git as a single source of truth for declarative infrastructure and applications. With Git at the center of your delivery pipelines, developers can make pull requests to accelerate and simplify application deployments and operations tasks to Kubernetes."*

## Flux: The GitOps Kubernetes Operator

- Ensures that the state of a cluster matches the config in Git
- Uses an operator in the cluster
- Monitors image repositories, detects new images, triggers deployments

![Flux CD Diagram](./assets/flux-cd-diagram.png)

- No separate CD tool
- No access to the cluster for CI tools
- Every change is atomic and transactional
- Git has the audit log

## Demo
