## Install Prerequisites:

 Change in /etc/sysctl.conf
 net.bridge.bridge-nf-call-iptables = 1
 net.bridge.bridge-nf-call-arptables = 1
 net.ipv4.ip_forward=1
 
 # Apply it using following
 sysctl -p 

 Restart romana-dns pod.

 Details about the issue: github.com/kubernetes/contrib/issues/2249

