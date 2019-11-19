# Difference between ACS, ACI and AKS


**Azure Container Instances (ACI)**

Azure container instance is a service on Azure that allows you to deploy container quickly. Azure Container Instances is a solution for any scenario that can operate in isolated containers, without orchestration. Run event-driven applications, quickly deploy from your container development pipelines, and run data processing and build jobs.

[With ACI, you can run docker containers on-demand in a managed serverless Azure environment.](https://docs.microsoft.com/en-us/azure/container-instances/)

Azure Container Instances is useful for scenarios that can operate in isolated containers, including simple applications, task automation, and build jobs. Here are some of the benefits:

    Fast startup: Launch containers in seconds.
    Per second billing: Incur costs only while the container is running.
    Hypervisor-level security: Isolate your application as completely as it would be in a VM.
    Custom sizes: Specify exact values for CPU cores and memory.
    Persistent storage: Mount Azure Files shares directly to a container to retrieve and persist state.
    Linux and Windows: Schedule both Windows and Linux containers using the same API.

For scenarios where you need full container orchestration, including service discovery across multiple containers, automatic scaling, and coordinated application upgrades, we recommend Azure Kubernetes Service (AKS).
