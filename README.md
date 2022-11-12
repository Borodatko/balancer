Nginx Balancer Playbook
=======================

This playbook set up and run load balancing test bench for two web servers.


Dependencies
------------

 - 4 VMs: 2 - webservers, 2 - LB;
 - RHEL family OS, version 8;
 - Python version 3.9.


Variables
---------

| Name | Description | Default Value |
|------|-------------|---------------|
| vrrp_interface | interface that vrrp runs on | enp0s3 |
| vrrp_pass | authentication password | CHANGEME |
| vrrp_addr | virtual address | CHANGEME |
| lb_ip01 | ip address of the primary LB node | CHANGEME |
| lb_ip02 | ip address of the secondary LB node | CHANGEME |
| srv01 | dns name of the first webserver | CHANGEME |
| srv02 | dns name of the second webserver | CHANGEME |
| srv01_ip | ip address of the first webserver | CHANGEME |
| srv02_ip | ip address of the second webserver | CHANGEME |
| tls | tls version, you can add versions separated by space | TLSv1.3 |
| ssl_path | path to certs & keys | /etc/ssl/certs |


License
-------

BSD-3-Clause


Author Information
------------------

https://github.com/Borodatko
