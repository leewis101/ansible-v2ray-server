Ansible Role: v2ray server
=========

Install v2ray server on linux.

Role Variables
--------------

| Name | default | description |
| ---- | ------- | ----------- |
| v2ray_version | latest | v2ray_version, e.g. v4.22.1 |
| v2ray_group | v2ray | run v2ray servcie as group |
| v2ray_user | v2ray | run v2ray service as user |
| v2ray_unpack_dir | /tmp/v2ray | location unpack v2ray.xxx.zip |
| v2ray_install_dir | /usr/local/v2ray | v2ray binarires install location |
| v2ray_config_dir | /etc/v2ray | v2ray configuration location |
| v2ray_log_dir | /var/log/v2ray | v2ray log location |

Example Playbook
----------------

Plase use your own `config.json.j2` before deployment.

```
$ ansible-galaxy install leewis101.ansible_v2ray_server
```

```yaml
- hosts: all
  roles:
    - leewis101.ansible-v2ray-server
```

License
-------

MIT
