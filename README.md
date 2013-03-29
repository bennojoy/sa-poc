### NIS sample

The functionalities of this playbook includes.

1) Deploy NIS servers and clients

2) Monitor and report the status of the yp server process.

3) Manage two maps of NIS Server, user and hosts.
   To add hosts to the nis map, just add the server to nis_vars/hosts and run the playbook playbook/addhost_ypserv.yml
   To add users to the nis map , just add the user to nis_vars/users and run the playbook playbook/adduser_ypserv.yml

   The advantage of keeping the whole inventory of nis users/hosts in ansible is that in case if disaster recovery, A fully configured NIS se   rver can be rebuilt in few minutes time.

4) Enforcing Security compliance of nis clients to ensure they dont send broadcasts and bind only to master server. (/etc/yp.conf)

Pending:

Updates to OS.
   
