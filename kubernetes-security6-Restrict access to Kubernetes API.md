Restrict Access to Kubernetes API
<img width="1556" height="839" alt="image" src="https://github.com/user-attachments/assets/b654d6b8-2eff-4fed-b034-d707e1563744" />
localhost:8001/api/v1/namespaces/test/pods
restrict the api server in 2 ways \
1)secure API server \
Anonymous requests to API \
2) secure kubernetes API server Ports&Ips \
By Default k8s serves HTTP on 2 diff ports \
8080 & 6443 \
<img width="1600" height="952" alt="image" src="https://github.com/user-attachments/assets/4142c589-1c1f-49c2-bb5d-523b73b4c830" />

Disable Anonymous requests to API \
API server level --anonymous-auth=true is its enabled \

there is one more authentication for the kubelet authentication
