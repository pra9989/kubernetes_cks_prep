Kubernetes Security - Restrict a Container's Syscalls with seccomp - 10
System Hardening \
SECCOMP LINUX SYS CALLS \
<img width="619" height="672" alt="image" src="https://github.com/user-attachments/assets/87c72ff6-c696-44e4-bf43-648edf08047e" />

Restricting the syscalls to resources \
Linux capabilities (clock_adjtime, mount, unmount, openat, fcntl...etc) sandbox priviligies \
Objective is to secure/restricting containers what are allowed to do \
Configured through profiles \
seccomp profile -- list syscalls to allow/deny/audit \
seccomp profiles - enabled at kublet level config (disable by default) \
Enable SecComp using kubelet config \
--feature-gates=SeccompDefault=true \
<img width="1606" height="869" alt="image" src="https://github.com/user-attachments/assets/75034485-9b47-46f5-9cad-7628033cec00" />
<img width="1632" height="967" alt="image" src="https://github.com/user-attachments/assets/6146a281-c21b-479f-a362-e4fb34c96b71" />
<img width="1610" height="958" alt="image" src="https://github.com/user-attachments/assets/a399da19-0f90-475c-ab2b-5bb34a03832b" />
Apply to POD \
spec:
  securityContext:
    seccompProfile:
      type: localhost
      localhostprofile: profiles/audit.json
  containers:
  - name: test-container
    image: hashicorp/http-echo:1.0
    args:
    - "-text=just made some more syscalls!"
    securityContext:
      allowPrivilegeEscalation: false \     
Types: localhost, RuntimeDefault, unconfined \
config path of seccomp profiles \
/var/lib/kubelet/   create a directory  mkdir seccomp/profiles \
/var/lib/kubelet/seccomp/profiles \
path to see the logs location when audit /var/log/sys \



