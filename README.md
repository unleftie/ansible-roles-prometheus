# Ansible Roles for Prometheus setup

[![CI](https://github.com/unleftie/ansible-roles-prometheus/actions/workflows/ci.yml/badge.svg)](https://github.com/unleftie/ansible-roles-prometheus/actions/workflows/ci.yml)
[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/unleftie/ansible-roles-prometheus/badge)](https://securityscorecards.dev/viewer/?uri=github.com/unleftie/ansible-roles-prometheus)

## Compatibility

| Platform | Version |
| -------- | ------- |
| debian   | 12      |

## Dependencies

- [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) (v2.14+)
- [Molecule](https://molecule.readthedocs.io/en/latest/installation.html) + (v4.0.4+) + [docker plugin](https://github.com/ansible-community/molecule-plugins) (for local testing)
- [Docker](https://docs.docker.com/get-docker/) (for local testing)

## Local Testing

```sh
git clone https://github.com/unleftie/ansible-roles-prometheus.git
cd ansible-roles-prometheus/roles/prometheus # or any other role
molecule test
```

## Installation

> Upgradability notice: When upgrading from old version of this role, be aware that some files may be lost.

Example [playbook](main.yml)

## 📝 License

This project is licensed under the [Apache License](LICENSE).
