# ansible-docker-ubuntu

[![Build Status](https://travis-ci.org/suzuki-shunsuke/ansible-docker-ubuntu.svg?branch=master)](https://travis-ci.org/suzuki-shunsuke/ansible-docker-ubuntu)

ansible role to install docker on Ubuntu.

https://galaxy.ansible.com/suzuki-shunsuke/docker-ubuntu/

## Requirements

Nothing.

## Role Variables

name | required | default | description
--- | --- | --- | ---
docker_version | no | latest | installed docker version
docker_state | no | do nothing | the state of docker daemon
docker_enabled | no | do nothing | whether docker daemon is enabled
docker_users | no | [] | users who are added the docker group

## Dependencies

Nothing.

## Example Playbook

```yaml
- hosts: servers
  roles:
  - role: suzuki-shunsuke.docker-ubuntu
    docker_users:
    - ubuntu
    become: yes
```

## License

[MIT](LICENSE)
