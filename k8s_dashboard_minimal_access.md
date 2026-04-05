Minimize use of, and access to GUI elements using RBAC \
Kubernetes Dashboard Access \
kubeconfig  \
token \
kubectl proxy \
Starting to serve on 127.0.0.1:8001 \
<img width="1578" height="922" alt="image" src="https://github.com/user-attachments/assets/f9d93792-09d3-4607-8b05-64e3a403d7be" />

STEP1: Create a service acccount with sample user \
STEP2: Create a cluster role --verb=get,list,watch --resource=pods,deployments,serices,configmaps \
STPE3: Bind the cluster role for cluster binding  kubectl create clusterrolebinding sample_binding --clusterrole=sample_role --serviceaccount=<namespace:serviceaccount_name>


<img width="729" height="478" alt="image" src="https://github.com/user-attachments/assets/ab77864a-2f90-448b-ac42-5cc2d54b11b0" />

Another way to access the kubernetes dashboard is bearer token \
USER_TOKEN=${kubectl get secret sample_secret -n sample_ns -o json | jq -r '.data["token"]' | base64 -d } \
echo $USER_TOKEN \
Then Set Credentials \
kubectl config set-credentials sample_user --token="$USER_TOKEN" \
kubectl config set-context <cluster-role> --cluster=<cluster-name from kubeconfig> --user <sample-user> \
So now you switch the create context and then check the permisssons which are allowed to tat specific user or working or not? 



