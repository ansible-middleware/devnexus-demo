# devnexus-demo

## Prerequisites

* We need Red Hat Enterprise Linux (RHEL) 9 two hosts subscribed to customer portal, one for Wildfly and another one for Quarkus

### Install Ansible Dependencies

`ansible-galaxy collection install -r requirements.yml`

## Running the demo

1. Execute the main play, run the all.yml file, which will setup the wildfly and quarkus will all the required configurations.


`ansible-playbook -i inventory/demo playbooks/demo.yml`

2. Once the playbook run is completed, you can access "http://localhost:9000/prices.html".

## License

Apache License v2.0 or later

See [LICENCE](LICENSE) to view the full text.


## Authors

* Harsha Cherukuri <hcheruku@redhat.com>
