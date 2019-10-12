#About Kubernates

Kubernetes (commonly stylized as k8s) is an open-source container-orchestration system for automating application deployment, scaling, and management. It was originally designed by Google, and is now maintained by the Cloud Native Computing Foundation. It aims to provide a "platform for automating deployment, scaling, and operations of application containers across clusters of hosts".It works with a range of container tools, including Docker. Many cloud services offer a Kubernetes-based platform or infrastructure as a service (PaaS or IaaS) on which Kubernetes can be deployed as a platform-providing service. Many vendors also provide their own branded Kubernetes distributions.

##Kubernates Features

* Endpoint Slices
  Scalable tracking of network endpoints in a Kubernetes cluster.
  
* Service discovery and load balancing
  No need to modify your application to use an unfamiliar service discovery mechanism. Kubernetes gives Pods their own IP addresses and a single DNS name for a set of Pods, and can load-balance across them.
  
* Automatic bin packing
  Automatically places containers based on their resource requirements and other constraints, while not sacrificing availability. Mix critical and best-effort workloads in order to drive up utilization and save even more resources.
  
* Storage orchestration
  Automatically mount the storage system of your choice, whether from local storage, a public cloud provider such as GCP or AWS, or a network storage system such as NFS, iSCSI, Gluster, Ceph, Cinder, or Flocker.
  
* Self-healing
  Restarts containers that fail, replaces and reschedules containers when nodes die, kills containers that don’t respond to your user-defined health check, and doesn’t advertise them to clients until they are ready to serve.
  
* Automated rollouts and rollbacks
  Kubernetes progressively rolls out changes to your application or its configuration, while monitoring application health to ensure it doesn’t kill all your instances at the same time. If something goes wrong, Kubernetes will rollback the change for you. Take advantage of a growing ecosystem of deployment solutions.
  
* Secret and configuration management
  Deploy and update secrets and application configuration without rebuilding your image and without exposing secrets in your stack configuration.
  
* IPv4/IPv6 dual-stack
  Allocation of IPv4 and IPv6 addresses to Pods and Services

* Batch execution
  In addition to services, Kubernetes can manage your batch and CI workloads, replacing containers that fail, if desired.

* Horizontal scaling
  Scale your application up and down with a simple command, with a UI, or automatically based on CPU usage.

##Architecture
  
  Kubernetes follows the primary/replica architecture. The components of Kubernetes can be divided into those that manage an individual node and those that are part of the control plane.
  
  ###Kubernetes control plane
  The Kubernetes master is the main controlling unit of the cluster, managing its workload and directing communication across the system. The Kubernetes control plane consists of various components, each its own process, that can run both on a single master node or on multiple masters supporting high-availability clusters.
  
  ###Kubernetes node
  A Node, also known as a Worker or a Minion, is a machine where containers (workloads) are deployed. Every node in the cluster must run a container runtime such as Docker, as well as the below-mentioned components, for communication with the primary for network configuration of these containers.
  
  ###Add-ons
  Add-ons operate just like any other application running within the cluster: they are implemented via pods and services, and are only different in that they implement features of the Kubernetes cluster. The pods may be managed by Deployments, ReplicationControllers, and so on. There are many add-ons, and the list is growing.




     