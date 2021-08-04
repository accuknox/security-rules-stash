# Rules
Container daemon socket bind mounts allows access to the container engine on the node. This access can be used for privilege escalation and to manage containers outside of Kubernetes, and hence should not be allowed.

## Rule1
The  '/var/run/docker.sock' should be audited 

## Rule2
The  '/var/run/containerd.sock' should be audited 

## Rule3
The  '/var/run/crio.sock' should be audited 

### Severity
<p style='color:orange'><b>Medium</b></p>


### Configuration
NA

### Applicability
Host, Container

### Policy Engine
KubeArmor

### Action
Audit, Enforce