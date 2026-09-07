# Ansible Role for Prometheus exporters

[![CI](https://github.com/unleftie/ansible-roles-prometheus/actions/workflows/ci.yml/badge.svg)](https://github.com/unleftie/ansible-roles-prometheus/actions/workflows/ci.yml)
[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/unleftie/ansible-roles-prometheus/badge)](https://securityscorecards.dev/viewer/?uri=github.com/unleftie/ansible-roles-prometheus)

Thin wrapper role that applies the [prometheus](https://github.com/prometheus-community/ansible) roles from the upstream
[prometheus.prometheus](https://galaxy.ansible.com/ui/repo/published/prometheus/prometheus/) collection. Override variables live in `vars/` directory, one file per role.

## Compatibility

| Platform | Version |
| -------- | ------- |
| ubuntu   | 26.04   |

## Dependencies

- [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) (v2.14+)
- [Molecule](https://molecule.readthedocs.io/en/latest/installation.html) + (v4.0.4+) + [docker plugin](https://github.com/ansible-community/molecule-plugins) (for local testing)
- [Docker](https://docs.docker.com/get-docker/) (for local testing)

## Local Testing

```sh
git clone https://github.com/unleftie/ansible-roles-prometheus.git
cd ansible-roles-prometheus
ansible-galaxy install -r requirements.yml
molecule test
```

## Installation

```sh
ansible-galaxy install -r requirements.yml
```

Example [playbook](main.yml)

## Documentation

- [Molecule tests](docs/molecule-testing.md)

## 📝 License

This project is licensed under the [MIT](LICENSE).
