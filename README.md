	Worker Node or Data Pane	

	Conatainer Runtime responsbility-  creates container runtime to run the container
		- Kubernetes: Container-D, cri-o, Dockerswam- support any other container runtime ($)
		- Docker: Dockerswam ($Docker run)

	Kubelete: Pod responsibility- responsible for creatin of pods and its running.

	kube-proxy: Networkig responsbility- use IP table and assign IP addrs to pod and load balancing capability for pod. 
		- in docker: Docker 0 present for networking called bridge networking.


					Master Node or Control Pane

	API Server: Exposes kubernets services to external world. user interact with it.

	Shedular: take request from API server and Shedules pods on nodes

	Etcd: Store entire kubernetes cluster information in the form of key value pair.

	Controller Manager: Inbuilt Manager-responsible for maintaining and controlling a specific aspect of the cluster, 
			ensuring that the desired state is achieved and maintained. 
			Node desired state, number of replica for a set of pods etc.

	Cloud Controller Manager: It is open source. Build for Cloud- Cloud made changes in it and  use to implements kubernetes services on cloud like EKS on AWS.
			It serves as an interface between the generic Kubernetes control plane components and the cloud provider's APIs, 
			allowing Kubernetes to manage resources and services provided by various cloud providers.
			like load balancers, block storage, and networking. ELBs, EBS, Auto scaling group are CCM in AWS.
 
