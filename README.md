# Role Name
=========

Install and Configure the Home Assistant application in a docker container

## Requirements
------------

Docker should already be installed on the host, the `geerlingguy.docker` Ansible role is a suitable solution.

## Role Variables
--------------

See the [comment in the default variables file](defaults/main.yml) for information

## Dependencies
------------

```collections
 - community.docker```

## Example Playbook
----------------
    - hosts: docker
      roles:
        - name: homeassistant
          when: '"homeassistant" in containers'
          tags: [ homeassistant, docker_up ]

## License
-------

BSD

