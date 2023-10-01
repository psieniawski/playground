Change vm limits on worker nodes

https://www.elastic.co/guide/en/elasticsearch/reference/current/vm-max-map-count.html

`sysctl -w vm.max_map_count=262144`

or

To set this value permanently, update the vm.max_map_count setting in /etc/sysctl.conf. To verify after rebooting, run `sysctl vm.max_map_count`.

[Installation instructions](https://www.elastic.co/guide/en/elasticsearch/reference/8.10/docker.html)

    docker-compose -f elastic-kibana.yaml up --detach

Kibana URL: `http://<docker-host>:5601` Username and password in .env file.