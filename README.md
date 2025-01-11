# Ansible Role: EPEL

Installs the EPEL repository (Extra Packages for Enterprise Linux) for RHEL/CentOS.

## Requirements

RedHat/CentOS

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```yaml
epel_version: "{{ ansible_distribution_major_version }}"
epel_package_url: "https://dl.fedoraproject.org/pub/epel/epel-release-latest-{{ epel_version }}.noarch.rpm"
epel_gpg_key_url: "https://dl.fedoraproject.org/pub/epel/RPM-GPG-KEY-EPEL-{{ epel_version }}"
```

## Dependencies

None

## Example Playbook

```yaml
- hosts: all
  roles:
    - { role: farisc0de.epel }
```

## License

MIT
