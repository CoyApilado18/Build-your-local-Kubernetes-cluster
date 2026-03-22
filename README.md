# This K8s install are beneficial for those learning Kubernetes. This is so useful if you're taking up CKA, CKAD, CKS. You can even use this as a lab to test your yaml files before deploying to cloud eg: EKS, AKS, GKE as there are costs when spinning up a k8s cluster into these cloud providers. 

# The instructions.txt are for setting up a multi-node cluster, which means the controlplane and the worker node are two different machines. First, set up the controlplane node and then run the kubeadm join command on the worker node to join the cluster.

# Prerequisites 
- Install your preferred VM software (eg: VirtualBox, VMware, Proxmox) and create two VMs for the controlplane and worker node.
- A compatible linux host (eg: Ubuntu 22.04)
- At least 2GB of RAM per machine. 
- At least 2 CPUs for the controlplane.
- Full network connectivity between all machines.
- Commands are to be run as root or with sudo privileges on both controlplane and worker node, except for the part where I noted "do not run commands on the worker node". 
