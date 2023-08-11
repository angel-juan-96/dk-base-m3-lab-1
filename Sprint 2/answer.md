# Sprint 2
TODO: Student to complete code and comments in the sections below.

## Install Kubernetes node 2

- Results from kubeadm --join:


[34.218.45.26] (BINARY-N/A:N/A) k8s@hol12 ~
$ sudo kubeadm join 34.219.212.132:6443 --token wmru58.7r4i9cbcifsketsg --discovery-token-ca-cert-hash sha256:b1ccdb564d75ee1eb103fc193d59788e9238bc30aa4cd027bd62b90ce9695aa1
[preflight] Running pre-flight checks
[preflight] Reading configuration from the cluster...
[preflight] FYI: You can look at this config file with 'kubectl -n kube-system get cm kubeadm-config -o yaml'
[kubelet-start] Writing kubelet configuration to file "/var/lib/kubelet/config.yaml"
[kubelet-start] Writing kubelet environment file with flags to file "/var/lib/kubelet/kubeadm-flags.env"
[kubelet-start] Starting the kubelet
[kubelet-start] Waiting for the kubelet to perform the TLS Bootstrap...

This node has joined the cluster:
* Certificate signing request was sent to apiserver and a response was received.
* The Kubelet was informed of the new secure connection details.

Run 'kubectl get nodes' on the control-plane to see this node join the cluster.