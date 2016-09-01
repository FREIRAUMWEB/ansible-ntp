NTP
=========

Installs ntp service for time synchronization on Ubuntu Trusty / Xenial

Variables
---------

- ntp_servers: an Array of fqdn wich defaults to:
  - 0.pool.ntp.org
  - 1.pool.ntp.org
  - 2.pool.ntp.org
  - 3.pool.ntp.org

- ntp_driftfile: e.g. /var/lib/ntp/ntp.drift

- ntp_restricts: an Array of restricts wich defaults to
  - "default kod notrap nomodify nopeer noquery"
  - "-6 default kod notrap nomodify nopeer noquery"
  - "127.0.0.1"
  - "::1"


Example Playbook
----------------

An example of how to use this role in your own playbooks

    - hosts: servers
      roles:
         - FREIRAUMWEB.ntp

License
-------

MIT

Author Information
------------------

This role was created in 2016 by Andreas Kleindiek @ FREIRAUMWEB (http://www.freiraumweb.de)
