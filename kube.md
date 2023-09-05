# Kubernetes

1. What is Kubernetes, and how would you explain it to someone who has never heard of it before?

# answer 

imagine kubernetes as Container crane at the docks that move containers around loads them to ships to be sent away or keep them organised and ready 

2. Can you describe the basic components of a Kubernetes cluster (such as nodes and control plane) and their role?
 kubenete cluster has two sections

 # Control plane:

 -1 apiserver: is a component of the Kubernetes control plane that exposes the Kubernetes API.
 
 -2 etcd: highly available key value store used to store the all cluster data
 
 -3 kube-scheduler:watches for newly created Pods with no assigned node, and selects a node for them to run on.

 -4 kube-controller-manager: Control plane component that runs controller processes, there are several types of controllers (node controller, job controller, EndpointSlice controller, ServiceAccount controller)

 -5 cloud-controller-manager: a controller that it's job to link the cluster to the cloud provider selected.

# Node  

-1 kubelet: a component in each node that makes sure that containers are running in a Pod.

-2 kube-proxy: maintains network rules on nodes. These network rules allow network communication to the Pods from network sessions inside or outside of your cluster.

3. How does Kubernetes ensure high availability and fault tolerance of applications within a cluster?

Kubernetes employs several mechanisms and strategies to ensure high availability and fault tolerance such as:

  -1 Service Discovery and Load Balancing: Kubernetes provides built-in service discovery and load balancing. Services distribute incoming traffic across the healthy pods, ensuring that requests are routed to available instances of the application 

  -2 Auto-scaling: Kubernetes allows us to run multiple replicas of the application pods across different nodes in the cluster. If a node fails, the pods on that node can be rescheduled to healthy nodes automatically.

  -3 self-healing: the state of pods is always monitored by the cluster. If a pod failed it's then replaced by another healthy pod.  

  -4 Backups: Implementing a regular backups of the cluster's data in case of malfunction 

4. What is a Kubernetes Service, and why is it important for networking and communication between Pods?

  service is a group of pods that enable to expose them to interaction with the internet providing fault tolerance, and load balancing, in other words it's to manage pods


5. What is a Pod in Kubernetes, and why is it a fundamental building block for containerized applications?

  pods are the smallest unit that can be created and managed in kubernetes, they are important because kubernetes manages 
containers through them.