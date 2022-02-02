# Ansible Role: Chrony

This role enables users to install and configure chrony on their hosts.


## Requirements

None

## Examples

1) Install chrony and use the default settings.

```

- hosts: all
  roles:
    - role: manishjuneja.chrony
```

2) Install chrony and use custom servers.

```

- hosts: all
  roles:
    - role: manishjuneja.chrony
  vars:
    chrony_config_server:
      - 0.pool.ntp.org
      - 2.pool.ntp.org
```
