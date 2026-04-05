System Hardening \
Kubernetes Security - Restrict Container Access with AppArmor - 9 \
AppArmor \
Linux Sys calls \
Restrict Container ACcess to resources \
A kernel level security for the containers linux capabailities, network access, file permissions etc \
Objective is to secure/restricting containers what are allowed to do \
Configured through profiles \
AppArmor profile - set of rules \
Load the Prodile in kernel \
AppArmor Profile loaded in 2modes \
Enforce mode \
Complain Mode\
AppArmor Implementation \
   > Install AppArmor \
   > Create Profile \
   > Enforce/load AppArmor Profiles  [we need to deploy on all the nodes] \
   > Apply profile to pod \
   > Containers & system are secured \
Apply to the pod using add annotations \
commands of apparmor sudo systemctl status apparmor \
> 
apparmor modeules are enabled or not cat /sys/module/apparmor/parameters/enabled \
<img width="1387" height="963" alt="image" src="https://github.com/user-attachments/assets/59156940-6a20-4229-ac65-563f5ab608e7" />

