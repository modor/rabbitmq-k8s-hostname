# rabbitmq-k8s-hostname

* The [rabbitmq-peer-discovery-k8s](https://github.com/rabbitmq/rabbitmq-peer-discovery-k8s/tree/master/examples/k8s_statefulsets) examples provide the yaml to create rabbitmq autocluster on k8s. But it is ip mode. When the rabbitmq store the data, it use ip as a data catalog name. When the pod recreated, name will be changed, and the data cannot be reused.
* This yaml provide the hostname mode to create rabbitmq autocluster on k8s. It solves the problems that data cannot be reused.
* Replace the 域名后缀 as your domain name, for example: rabbitmq-service.default.svc.cluster.local
