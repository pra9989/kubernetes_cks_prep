 Verify platform binaries before deploying 
1) Verify the kubernetes binaries using the checksum \
kubernetes binaries \
   > generate sha512 checksum \
   > compare/validate with offical release checksum \
kubernetes release page for the specific release
Go to the master node 
Download the binary from the kubernetes release page of changelog to the master node
sha512sum kubernetes-client-darwin-arm64.tar.gz 
<img width="1877" height="107" alt="image" src="https://github.com/user-attachments/assets/1cdd104d-d7c1-4994-a60f-a77b3a3f248a" />
method1:
so now go to the kubernetes changelog site and compare the sha number and validate  this is one method \
method2: 
   > If we want to check our kubectl installed is with preoper checksum or not \
   > go to the offical k8s website and download the checksum on kubectl node \
   > echo "$(<kubectl.sha256) /usr/bin/kubectl" | sha256sum --check \
   /usr/bin/kubectl: OK
   





