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


![k3d-demo](https://github.com/user-attachments/assets/284d2cfc-58ca-4811-9ca2-c6daf8f63a06)
