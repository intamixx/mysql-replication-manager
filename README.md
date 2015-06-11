# mysql-replication-manager

Manages several mysql slaves in a standard master slave setup using ansible.  For ease can be launched in dialog gui mode.

-u user configured for ansible use
-l list configured slaves. Used with -g to specify group of hosts
-g host group name configured in ansible
 -s <hosts> performs a stop, change master and start on the slave
  -b forces a copy and re-import of the database from master to the slave
  -r forces slave reset
  -m creates replication user on master
 -c <hosts> checks the slave replication
 -a checks the slave replication (report style). Used with -g to specify group of hosts
 -f start slave if not running
 -x Run tools in dialog mode
-d debug mode
