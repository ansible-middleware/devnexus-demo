# devnexus-demo

## Prerequisites

* Provision multiple Red Hat Enterprise Linux Hosts to support Wildfly Application Server and Quarkus based Application

* Install and Configure Wildfly Application Server with a JMS queue to process messages sent from applications

* Deploy and configure Quarkus based application

* Enable systemd services for native Operating System runtime management

### Install Ansible Dependencies

`ansible-galaxy collection install -r requirements.yml`

## Running the demo

1. Update the inventory file inventory/demo and update wildfly_vm_ip wth the ip address of wildfly instance in inventory/group_vars/quarkus.yml. Execute the playbook all.yml to setup the demo, which will setup the wildfly and quarkus will all the required configurations.

`ansible-playbook -i inventory/demo playbooks/demo.yml`

2. Once the playbook run is completed, you can access "http://<replace with quarkus_ip or localhost>:9000/prices.html".

## License

Apache License v2.0 or later

See [LICENCE](LICENSE) to view the full text.


## Authors

* Harsha Cherukuri <hcheruku@redhat.com>
