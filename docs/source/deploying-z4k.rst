Deploying Zerto for Kubernetes
==============================

In a Kubernetes environment, Zerto for Kubernetes is installed and designed to protect next generation applications. 

The installation includes the following: 

* Zerto Kubernetes Manager (ZKM): A containerized application that manages everything required for the replication between the protected and recovery clusters, apart from the actual replication of data. ZKM interacts with ZKM-PX as its proxy to a Kubernetes cluster and VRAs in order to orchestrate replication. ZKM manages the entire environment and therefore it is required to have only one instance of it. 

* Zerto Kubernetes Manager Proxy (ZKM-PX): A containerized application which serves as a communication proxy between the Kubernetes cluster and the VRA. Zerto requires one ZKM-PX installed per cluster. 

* Virtual Replication Appliance (VRA): A containerized application which is automatically installed on each cluster node. VRAs manage the replication of data from containers to the recovery cluster. 

* Networking: When replicating between clusters, Zerto requires ingress to manage all cross cluster communication. If replication is done within the same cluster, there is no need for this component. 

* Keycloak: Keycloak is an open source identity and access management tool which is used for user and component authentication. It is deployed automatically as part of the ZKM installation, and only one instance is required. 

* Zerto Analytics: A Zerto user interface which provides a view over all existing VPGs. For deployment prerequisites, installation instructions, and initial use, [click here]. 

[click here]: ./usage