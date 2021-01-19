# Ansible Role: pyMedusa

A role that installs [pyMedusa](https://pymedusa.com/)

## Requirements

None.

## Role Variables

```
# The Medusa data dir.
# You might want to change this when running on (for example) a raspberry pi.
pymedusa_directory: "/opt/medusa"

# The Linux user to run the medusa service as.
pymedusa_service_user: "medusa"

# The Linux user group to run the medusa service as.
pymedusa_service_group: "medusa"

# The pymedusa options for config.ini
pymedusa_options:
  - { section: 'General', option: 'backup', value: true }
```

## Dependencies

None.

## Example Playbook

```
- hosts: servers
  roles:
     - jelle_s.pymedusa
```

## License

[MIT](https://raw.githubusercontent.com/Jelle-S/ansible_role_pymedusa/master/LICENSE)

