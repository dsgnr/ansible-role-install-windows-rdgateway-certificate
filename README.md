# Ansible Role: Windows Install RDGateway Certificate

[![Build Status](https://travis-ci.org/dsgnr/ansible-role-install-windows-rdgateway-certificate.svg?branch=master)](https://travis-ci.org/dsgnr/ansible-role-install-windows-rdgateway-certificate)

Imports and assigns a certificate to the RDGateway

## Requirements

None.

## Role Variables

certificate_tld: "example.com"

broker_subdomain: "rds"

## Dependencies

None.

## Example Playbook

    - hosts: RDGateway
        vars:
          certificate_tld: example.com
          broker_subdomain: bts
      
      roles:
        - install-windows-rdgateway-certificate

## Example task command

```
    ansible-playbook -l RDGateway install-windows-rdgateway-certificate.yml -e "certificate_tld=example.com broker_subdomain=rds"
```

## License

GNUv3
