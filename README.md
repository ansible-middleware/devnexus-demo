# devnexus-demo

## Prerequisites

* Red Hat Enterprise Linux (RHEL) 8 host
* Ansible >= 2.9 / python >= 3.9

### Install Ansible Dependencies

`ansible-galaxy collection install -r requirements.yml`

## Running the demo

1. From the playbook run the qpid.yml which will setup the Apache Qpid server and start on the port 9080

`ansible-playbook -i inventory playbooks/qpid.yml`

2. Execute the main play, run the all.yml file, which will setup the wildfly and quarkus will all the required configurations.


`ansible-playbook -i inventory playbooks/all.yml`

3. Once the playbook run is completed, you can access "http://localhost:8090/prices.html" where you can pull the latest queue information.

## License

Apache License v2.0 or later

See [LICENCE](LICENSE) to view the full text.


## Authors

* Harsha Cherukuri <hcheruku@redhat.com>
