# librenms and oxidized
This playbook installs librenms and oxidized on a single host. 

Initial setup:

```
Librenms Username: admin
Librenms Password: admin
```

oxidized service is deactivated and needs to be enabled with ```systemctl enable oxidized.service --now```

This playbook applies against a plain CentOS 7 installation only. 

Use with ```ansible-playbook -i <inventory> install.yml```

Bugs to fix: 

* Use variables for database configuration
* Secure the installed mysql database
* Use a different snmp community for localhost 
