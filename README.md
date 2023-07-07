Homebox
=========

Homebox is the inventory and organization system built for the Home User.

This Ansible role installs Homebox as a Docker service.

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):


```
homebox_image: "ghcr.io/hay-kot/homebox:latest"
```
The version of the docker image to run as a container.

```
homebox_host_port: 7745
```
Homebox host port

```
homebox_host_config_path: /etc/homebox
```
Host path which stores homebox configuration.

```
homebox_host_data_path: /var/lib/homebox
```
Host path which stores homebox data.

```
homebox_timezone: "Europe/Madrid"
```
Timezone.

```
homebox_container_user: homebox
```
user running the container.

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - iasensio.homebox

License
-------

MIT

