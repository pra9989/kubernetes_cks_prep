Kubernetes Security - Open Policy Agent - OPA Gatekeeper - 12 \
Minimie Microservice vulnerabilities \
<img width="1606" height="701" alt="image" src="https://github.com/user-attachments/assets/74ec4269-9edf-47e2-b2fd-1b48cb1e7514" />
<img width="1624" height="818" alt="image" src="https://github.com/user-attachments/assets/5cdd9ed3-5862-4e46-b1bc-df769a56f191" />
<img width="1627" height="995" alt="image" src="https://github.com/user-attachments/assets/42ac297d-ad4c-4a90-85d0-7bd174ae5c3a" />
STEPS   FOR MUTATING WEBHOOKCONFIGURATION \
1) Deploy a webhook service (webserver) using svc (anyresource of k8s) \
2) Deploy MutatingWebhookConfiguration Yaml \
   <img width="1638" height="888" alt="image" src="https://github.com/user-attachments/assets/d90992da-3bb8-478e-91e3-68970ec099a1" />

Validating Webhook COnfiguration \
<img width="1490" height="942" alt="image" src="https://github.com/user-attachments/assets/9f2c2b29-3eb4-450b-92e3-4983d3683ab6" />
OPA is policy enforcement using high-level declarative language for microservices, k8s, CI/CD pipelines, API gateways and cloud native etc \
OPA GateKeeper allows you to enforce custome policies on any kubernetes object at creation time \
All images must be from approved repositories \
All ingress hostnames must be globally unique \
All pods must have resource limits \
All namespace must have a label that lists a point of contact \
GateKeeperv3.0 - The admission controller is integrated declarative policy support, validating, mutating admission control and audit control. \
Implement using policy templates which uses rego, CRDS, etc \
OPA Gatekeeper 3.0 for K8s \
Validating Admission control \
policies and constraints \
Audit \
Data Replication \
<img width="901" height="431" alt="image" src="https://github.com/user-attachments/assets/5c205cfb-d3d3-428f-866b-f8b33683b5e5" />
OPA Gatekeeper Implementation \
On K8s Cluster we need to install gatekeeper, create constraint template(Rego), Create constraint CRD, Create deploy && test constraint, Observe the enforcement \
<img width="1159" height="970" alt="image" src="https://github.com/user-attachments/assets/4c4753ff-5a25-48a5-89ad-f6cfbf751e5b" />
Constraint \
<img width="1577" height="992" alt="image" src="https://github.com/user-attachments/assets/9ae64480-8cae-4eae-81f4-3c820c6d6ac9" />
Audit - Data Replication \
<img width="1526" height="984" alt="image" src="https://github.com/user-attachments/assets/949bd238-d226-494e-a401-a0fa883c2455" />
<img width="593" height="277" alt="image" src="https://github.com/user-attachments/assets/3bcebbda-8307-4921-982c-f78bb7ae9f57" />






