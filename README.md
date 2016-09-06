haproxy-consul Role
=========

Configure and start haproxy-consul[1] in a docker container using the image `indigodatacloud/haproxy-consul:latest`. 

[1] https://github.com/CiscoCloud/haproxy-consul

Role Variables
--------------

- `haproxy_consul_mode` (default: marathon)
- `haproxy_consul_version` (default: latest)
- `haproxy_consul_image` (default: indigodatacloud/haproxy-consul:{{haproxy_consul_version}}) 


Dependencies
------------

- `indigo-dc.docker`

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: indigo-dc.haproxy-consul, haproxy_consul_mode: "marathon" }

License
-------

Apache Licence v2 [2]

[2] http://www.apache.org/licenses/LICENSE-2.0
