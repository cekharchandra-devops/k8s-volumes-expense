# Statefulset

* Cluster-IP service will return the virutal IP address assigned to it when `nslookup` the service name

* Service will loadbalance the endpoints(pods) attached to it. 

* Pod doesnt know about other replica pods of the same deployment using K8s Service.

* to know other pod's identity, head less service should be used.


**below are steps for creating statefulset for mysql**

* install ebs csi driver

* give csidriverpolicy permission to eks IAM role

* create ebs storage class

* create headless service along with service.

* create PVC