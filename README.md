# KubernetesCluster
Scripts for setting up master and worker nodes for a K8's cluster.

Master Node:
- Clone the master-node.sh in master node
- chmod +x master-node.sh (make executable)
- Installs Docker container run time 

Worker Node:
- Clone script worker-node.sh in worker node
- chmod +x worker-node.sh 
- Environment is setup


To join worker node to the cluster, we need a kubeadm command that will be generated at the master node
--> 'kubeadm token create --print-join-command' : run this command at the master node
--> Take the result and run it in worker node

IMP:
Also edit /etc/hosts file in all node and add all nodes in each node's file. Use the format given below
 192.168.8.215 node-1 <IP-addr> <hostname>

