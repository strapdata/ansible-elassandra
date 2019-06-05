# Elassandra Ansible Role

Elassandra Ansible role for Centos 7.x

## Requirements

* Synchronize system clocks
* Install TLS/SSL keystores and cacert.pem in /etc/cassandra
* Optimize disk settings
* Set rack accordingly with fault domains

## Role variables

See defaults/main.yml

## Dependencies

None

## Example Playbook

```yaml
---
- hosts: dc1
  become: yes
  roles:
    - elassandra
```

## Deploy elassandra

* Update your hosts file with your settings (see elassandra/defaults/main.yaml)
* Run ansible-playbook

```bash
ansible-playbook elassandra.yml -i hosts -v
```