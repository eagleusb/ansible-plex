[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/jonakoudijs/ansible-plex/Galaxy%20Publish?logo=github)](https://github.com/jonakoudijs/ansible-plex/actions)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-jonakoudijs.plex-blueviolet.svg)](https://galaxy.ansible.com/jonakoudijs/ansible_plex)
[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

# Plex Ansible Role

Install Plex on Linux (RedHat and Debian derivatives)

## Requirements

This role needs to be executed as root with `become: true`.

## Role Variables

The following variables are set in `defaults/main.yml` and can be overriden:

```yml
plex_repo: true  # (bool) Use official Plex package repository
plex_repo_key: "https://downloads.plex.tv/plex-keys/PlexSign.key"

plex_package_name: "plexmediaserver"
plex_package_state: "present"

plex_service_name: "plexmediaserver"
```

## Dependencies

This role does not have any dependencies.

## Example Playbook

Installing Plex:

```yml
- hosts: servers
  roles:
     - plex
```

## License

[MIT license](LICENSE)

## Author Information

Originally created by [Jona Koudijs](https://www.jona.io).
