Pod Security Policies (PodSecurityPolicy)
OS level security domain with podsecuritypolicies
Minimie Microservice vulnerabilities
How Admission controller will work in k8s
<img width="1592" height="779" alt="image" src="https://github.com/user-attachments/assets/56a82ab7-8c37-49e8-a9a9-1db14b73abfb" />
<img width="1625" height="989" alt="image" src="https://github.com/user-attachments/assets/ca66e847-fb39-4a53-8c8b-87707a02035c" />
PSP
Cluster level global resource(not namespaced)
control security sensitive aspects of the pod specification
set of conditions that a pod must run + defaults for the releated fields. \
Admins will configure PSP in cluster \
Must be enabled at kubeAPI server level before using it 
PodSecurityPolicy - can be authored using RBAC \
Pod Security Standards
Privilged \
Baseline \
Restricted \
Profile	Description \
Privileged	Unrestricted policy, providing the widest possible level of permissions. This policy allows for known privilege escalations. \
Baseline	Minimally restrictive policy which prevents known privilege escalations. Allows the default (minimally specified) Pod configuration. \
Restricted	Heavily restricted policy, following current Pod hardening best practices. \
https://kubernetes.io/docs/concepts/security/pod-security-standards/ \
Enable & Disable Admission controllers \
kube-apiserver level \
--enable-admission-plugins=PodSecurityPolicy \
<img width="1229" height="761" alt="image" src="https://github.com/user-attachments/assets/1db7d24c-6dcc-4123-bcf0-5c4f8dc87c9d" />
<img width="1649" height="1000" alt="image" src="https://github.com/user-attachments/assets/0638742f-45ab-4626-a6a6-af369ff61722" />



