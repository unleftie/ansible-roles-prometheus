# Ansible Role for Prometheus exporters

[![CI](https://github.com/unleftie/ansible-roles-prometheus/actions/workflows/ci.yml/badge.svg)](https://github.com/unleftie/ansible-roles-prometheus/actions/workflows/ci.yml)
[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/unleftie/ansible-roles-prometheus/badge)](https://securityscorecards.dev/viewer/?uri=github.com/unleftie/ansible-roles-prometheus)

Thin wrapper role that applies the `node_exporter`, `fail2ban_exporter`, and `nginx_exporter` roles from the upstream
[prometheus.prometheus](https://galaxy.ansible.com/ui/repo/published/prometheus/prometheus/) collection. Each exporter can be toggled
independently via `node_exporter_role_enabled` / `fail2ban_exporter_role_enabled` / `nginx_exporter_role_enabled` (default `true`) in
[defaults/main.yml](defaults/main.yml). Override variables live in [vars/](vars/), one file per exporter.

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

## 📝 License

This project is licensed under the [MIT](LICENSE).
