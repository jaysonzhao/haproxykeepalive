# Ansible Role: firewalld

![Ansible Galaxy](https://github.com/0x022b/ansible-role-firewalld/workflows/Ansible%20Galaxy/badge.svg)

Ansible role that configures firewalld package and service.

## Requirements

None.

## Role Variables

Available variables are listed below with default values.

```yaml
firewalld_package_state: present
```

Variable to control the state of firewalld package.

```yaml
firewalld_service_state: started
firewalld_service_enabled: yes
```

Variables to control the state of firewalld service.

```yaml
firewalld_default_interface: "{{ ansible_default_ipv4.interface }}"
firewalld_default_zone: public
```

Variables to control the default interface and zone.

## Dependencies

None.

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: 0x022b.firewalld
```

## Versioning

This project uses [Semantic Versioning][semver].

## License

MIT

[semver]: https://semver.org/
