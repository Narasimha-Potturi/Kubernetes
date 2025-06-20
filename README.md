# Architecure of the Kubernetes Simplified

### *Ever wondered Why you see K8s instead of kubernetes in some documentations.*

Here's the reason:

K8s is nothing but the shortened form of the word "Kubernetes".
The word "Kubernetes" has 8 Letters between the letters K and S . so in short it is called as K8S. People uses this as it much easier to read and type .


## Difference between Docker and Kubernetes

To better understand the Architecture of the Kubernetes, We have to understand the difference between the docker and kubernetes.

On a high level k8s offers you 4 Fundamental advanatages over the docker

1.Cluster

2.Autohealing

3.Autoscaling

4.Multiple Enterprise Level Support

What do Mean by Cluster?

Cluster is noting but a group of nodes together is called a cluster. Kubernetes in general is installed in a **Master Node Architecture** just like in Jenkins.

Advantages of Installing Kubernetes as a Cluster
1. **High Availability**: If one node goes down, the other nodes in the cluster can take over, ensuring that your applications remain available.
2. **Load Balancing**: Kubernetes can distribute the load across multiple nodes, improving performance and resource utilization.
3. **Scalability**: You can easily add or remove nodes from the cluster based on your needs, allowing for dynamic scaling of resources.
4. **Resource Management**: Kubernetes can efficiently manage resources across the cluster, optimizing the use of CPU, memory, and storage.
5. **Fault Tolerance**: If a node fails, Kubernetes can automatically reschedule the workloads to other healthy nodes, ensuring minimal downtime.

## Autohealing
Autohealing is a feature of Kubernetes that automatically detects and replaces failed containers or nodes in a cluster. This ensures that applications remain available and responsive, even in the face of hardware or software failures.
## Autoscaling
Autoscaling is a feature of Kubernetes that automatically adjusts the number of running instances of an application based on current demand. This ensures that applications can handle varying workloads efficiently without manual intervention.
## Multiple Enterprise Level Support
Kubernetes is a tool that was created by Google and is cncf maintains it. Docker is just a contaner platforma and is never used in production environments.  Kubernetes supports multiple container runtimes, including Docker, containerd, and CRI-O. This flexibility allows organizations to choose the best container runtime for their needs and easily switch between them if necessary.

## Understading various components of Control Plane and Data Plane

![ControlPlane & Date Plane](https://github.com/user-attachments/assets/48c59cb9-77e8-4be0-8d9d-c656578e1a19)
***NOTE*** Here for the better understanding, I have taken one master and two worker nodes. Where as in the real production environment you have multiple masters and multiple worker nodes.

### Control Plane

### *What is Control Plane?*

The control plane is the heart or the core component of the Kubernetes cluster. It manages the cluster's state, including scheduling, scaling, and maintaining the desired state of applications. The control plane consists of several components that work together to ensure the smooth operation of the cluster.
If you look at the image you could see control plane and data plane , Let's now try to see various components in the control plane.
**NOTE:** In k8s , whenever you request for a service or something with the application the request is not directly sent to the worker node, Insted what it does is
the request is sent to the worker node through the master, so here request always go through the master and that's why it is called as control plane means which controls.








