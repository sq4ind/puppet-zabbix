#wdijkerman-zabbix release

Below an overview of all changes in the releases.

Version (Release date)

0.2.0  (2014-06-18)

  * Added rspec test for zabbix::agent
  * Added rspec test for zabbix::repo
  * Added rspec test for zabbix::proxy
  * Added rspec test for zabbix::server
  * Added rspec test for zabbix::database{mysql,postgresql}
  * Added rspec test for zabbix::userparameters
  * Added rspec test for zabbix::javagateway
  * zabbix::userparameters fixed via pull request github (By 'suff')  --> Thanks!
  * Removed some documented settings
  * nodeid wasn't working with zabbix_server.conf template

0.1.0  (2014-04-17)

  * Added manage_repo parameter. If set to true, it will install the apt/yum repository.
  * Updated module for support Ubuntu (12.x).
  * Updated module for support Debian (6, 7).
  * Updated module for support Oracle Linux (5, 6).

0.0.3  (2014-03-31)

  * Added parameter: manage_vhost for creating vhost (Default: true)
  * Added parameter: manage_firewall for creating firewall rules
  * Added zabbix::javagateway class for installing the Zabbix Java Gateway
  * Renaming parameters javagateway_host to javagateway and javagateway_port to javagatewayport for zabbix::proxy (Same naming as the zabbix::server).

0.0.2  (2014-03-28)

  * MySQL can be used as database back-end.
  * Services started at boot.
  * Vhost creation, need 1 parameter for zabbix-server: zabbix_url.
  * Updated the readme.md

0.0.1 (2014-03-18)

  * Initial working version. Installing of the 
    * zabbix-server
    * zabbix-agent
    * zabbix-proxy
  * Possibility to add userparameters for the zabbix-agent.
