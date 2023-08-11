# Probar Kubernetes en nodo 1

Objetivos
- Crear namespace y pods monitoreando su estado con la modalidad watch

Tareas
Crear namespace, monitorear cambios a etiquetas en modalidad watch
Monitorear cambios a eventos de pods, crear pod de corta duración

$ kubectl get namespace hello -o yaml apiVersion: v1 kind: Namespace metadata: creationTimestamp: "2023-08-11T02:33:55Z" labels: kubernetes.io/metadata.name: hello name: hello resourceVersion: "2390" uid: 9b3da13a-c8af-4800-ab51-e43d357abc13 spec: finalizers:

kubernetes status: phase: Active [34.219.212.132] (kubernetes-admin@kubernetes:N/A) k8s@hol11 ~/.kube $ kubectl get namespaces --show-labels -w NAME STATUS AGE LABELS default Active 24m kubernetes.io/metadata.name=default hello Active 22s kubernetes.io/metadata.name=hello kube-node-lease Active 24m kubernetes.io/metadata.name=kube-node-lease kube-public Active 24m kubernetes.io/metadata.name=kube-public kube-system Active 24m kubernetes.io/metadata.name=kube-system
