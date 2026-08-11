# Ansible Roles for Grafana setup

[![CI](https://github.com/unleftie/ansible-roles-grafana/actions/workflows/ci.yml/badge.svg)](https://github.com/unleftie/ansible-roles-grafana/actions/workflows/ci.yml)
[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/unleftie/ansible-roles-grafana/badge)](https://securityscorecards.dev/viewer/?uri=github.com/unleftie/ansible-roles-grafana)

Thin wrapper role that applies [`grafana.grafana`](https://github.com/grafana/grafana-ansible-collection) roles from the upstream
[grafana.grafana](https://galaxy.ansible.com/ui/repo/published/grafana/grafana/) collection. Override variables live in [vars/main.yml](vars/main.yml)

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
git clone https://github.com/unleftie/ansible-roles-grafana.git
cd ansible-roles-grafana
ansible-galaxy install -r requirements.yml
molecule test
```

## Installation

```sh
ansible-galaxy install -r requirements.yml
```

Example [playbook](main.yml)

## 📝 License

This project is licensed under the [MIT](LICENSE).
