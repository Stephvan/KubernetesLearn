# Difference between ACS, ACI, AKS and ACR


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

**[Azure Kubernetes Service](https://docs.microsoft.com/en-us/azure/aks/)**

Azure Kubernetes (AKS) is a managed Kubernetes service. I.e. It manages your hosted Kubernetes environment, making it quick and easy to deploy and manage containerized applications without container orchestration expertise (you do not have to be an expert at orchestration to use Kubernetes if you employ yo use AKS)

You can call AKS the Azure Kubernetes Engine similar to Google Google Kubernetes Engine (GKE).

If you have never used Azure you will need to register a few providers namely for Compute, Network and Storage. The three steps below will do it but note that it may take a few minutes for the registration to complete:


```
$ az provider register -n Microsoft.Compute
$ az provider register -n Microsoft.Network
$ az provider register -n Microsoft.Storage
```

These providers can also be registered on [Azure portal](https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-manager-supported-services#azure-portal).


### [Azure Container Registry (ACR)](https://docs.microsoft.com/en-us/azure/container-registry/) ###
---

Azure Container Registry allows you to build, store, and manage container images and artifacts in a private registry for all types of container deployments.


#### Links and further reading: ####

[AZ, ACI, AKS, ACS in 5 minutes top chrono!](https://medium.com/bitnami-perspectives/az-aci-aks-acs-in-5-minutes-top-chrono-65c9952dfeb8) -- [Sebastien Goasguen](https://medium.com/@sebgoa)

[Azure Kubernetes Service (AKS](https://docs.microsoft.com/en-us/azure/aks/)

[Azure CLI for Container](https://docs.microsoft.com/en-us/cli/azure/container?view=azure-cli-latest#az-container-create)

[Microsoft Learn -- Introduction to Azure Container Instances](https://docs.microsoft.com/en-us/learn/modules/run-docker-with-azure-container-instances/1-introduction)

[Container Services](https://azure.microsoft.com/en-us/product-categories/containers/)

[Container Service (deprecated)](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/microsoft.acs)

[Container Service Documentation](https://docs.microsoft.com/en-us/azure/container-service/)

[Azure Container Registry documentation](https://docs.microsoft.com/en-us/azure/container-registry/)
