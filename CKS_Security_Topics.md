1. Cluster Setup - 10% \
1.1 Network security policies \
1.2 Install & Fix using kube-bench \
1.3 Ingress TLS termination \
1.4 Protect node metadata and endpoints with NetworkPolicy \
1.5 Minimize use of, and access to, GUI elements \
1.6 Verify platform binaries before deploying \
2. Cluster Hardening - 15% \
2.1 Restrict access to Kubernetes API \
2.2 Use Role-Based Access Controls to minimize exposure \
2.3 Exercise caution in using service accounts e.g. disable defaults, minimize permissions on newly created ones \
2.4 Update Kubernetes frequently \
3. System Hardening - 15% \
3.1 Minimize host OS footprint (reduce attack surface) \
3.2 Minimize IAM roles \
3.3. Minimize external access to the network \
3.4 Appropriately use kernel hardening tools such as AppArmor, seccomp \
3.4.1 SECCOMP PROFILES \
3.4.2 APPARMOR \
4. Minimize Microservice Vulnerabilities - 20% \
4.1 Setup appropriate OS level security domains e.g. using PSP, OPA, security contexts \
Admission Controller \
4.1.1 Pod Security Policies (PSP) \
4.1.2 Open Policy Agent (OPA) \
4.1.3 Security Contexts \
4.2 Manage Kubernetes secrets \
4.3 Use container runtime sandboxes in multi-tenant environments (e.g. gvisor, kata containers) \
4.3.1 gvisor \
4.3.4 kata containers \
Install gVisor \
Container Runtime \
4.4 Implement pod to pod encryption by use of mTLS \
5. Supply Chain Security - 20% \
5.1 Minimize base image footprint \
5.2 Secure your supply chain: whitelist allowed registries, sign and validate images \
5.3 Use static analysis of user workloads (e.g.Kubernetes resources, Docker files) \
5.4 Scan images for known vulnerabilities \
6. Monitoring, Logging and Runtime Security - 20% \
6.1 Perform behavioral analytics of syscall process and file activities at the host and container level to detect malicious activities \
6.2 Detect threats within physical infrastructure, apps, networks, data, users and workloads \
6.3 Detect all phases of attack regardless where it occurs and how it spreads \
6.4 Perform deep analytical investigation and identification of bad actors within environment \
6.5 Ensure immutability of containers at runtime \
6.6 Use Audit Logs to monitor access \
debugging api-server/kubelet failures \
