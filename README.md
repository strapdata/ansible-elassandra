# Elassandra Ansible Role

## Requirements

* Synchronize system clocks
* Install TLS/SSL keystores and cacert.pem in /etc/cassandra
* Optimize disk settings
* Set rack accordingly with fault domains

## Usage

* Update your settings in elassandra/defaults/main.yaml
* Update your hosts file

## Deploy elassandra

```bash
ansible-playbook elassandra.yml -i hosts -vvv -b
```
