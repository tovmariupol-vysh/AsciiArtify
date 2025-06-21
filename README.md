# AsciiArtify
### Comparison of three tools for deploying Kubernetes clusters in a local environment — minikube, kind, and k3d.

| Characteristics   |       minikube      |           kind           |            k3d           |
| ----------------- | ------------------- |------------------------- |------------------------- |
| Requirements      | 2 CPUs or more      | 2 CPUs or more per node  | 2 CPUs or more per node  |
|                   | RAM 2Gb or more     | RAM 4Gb or more per node | RAM 4Gb or more per node |
|                   | Disk 20Gb or more   | Disk 40Gb or more        | Disk 20Gb or more        |
| Support OS        | Linux,macOS,Windows | Linux,macOS,Windows      | Linux,macOS,Windows      |
| Architecture      | x86-64,ARM64,ARMv7, | AMD64,ARM64              | AMD64,ARM, ARM64,386     |
|                   | ppc64, S390x        |                          |                          |
| Monitoring        | dashboard           | dashboard                | dashboard                |
| CRI               | CRI-0, containerd,  | docker,podman,nerdctl    | docker,podman            |
|                   | docker              |                          |                          |
| Support podman    | experimental        | yes                      |  yes                     |
| Support multinode | no                  | yes                      |  yes                     |


All the proposed products allow you to deploy a Kubernetes cluster on local resources. However, Minikube can only work on a single node and does not support scaling the application across multiple nodes. Kind and k3d have approximately the same capabilities when deploying applications on a Kubernetes cluster.
For example, both products support high availability mode for both management nodes and worker nodes. Both also support the use of not only Docker but also Podman as container management tools. This is important, since there are licensing restrictions when using Docker.
But K3d is based on the K3s project, and Kind is based on the K8s project. Therefore, k3d uses fewer system resources, so the Kubernetes cluster is created and started faster. I recommend the startup "AsciiArtify" to choose the K3d option for deploying applications in a Kubernetes cluster.

I've added a demonstration of creating a Kubernetes cluster in k3d and deploying a simple "Hello world" application to the cluster.

![k3d-demo](https://github.com/user-attachments/assets/284d2cfc-58ca-4811-9ca2-c6daf8f63a06)
