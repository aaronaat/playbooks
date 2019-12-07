Useful ansible playbooks

install-package.yml **install latest package if no other version present**

snmp.yml **install list of packages, update configuration file, disable firewall**

resource-check.yml **check system resources**
```
:~/playbooks$ ansible-playbook resource-check.yml | grep msg > info.txt && cat info.txt
    "msg": "127.0.0.1"
    "msg": "CPU user:5.8 | system:2.5"
    "msg": "RAM free:1160 | used:6655 | total:7815"
    "msg": "Device /dev/loop0 free:0.0GB | total:0.0GB"
    "msg": "Device /dev/loop1 free:0.0GB | total:0.0GB"
    "msg": "Device /dev/loop3 free:0.0GB | total:0.0GB"
    "msg": "Device /dev/sda1 free:1.0GB | total:1.0GB"
    "msg": "Device /dev/mapper/ubuntu--vg-root free:459.0GB | total:501.0GB"
    "msg": "Device /dev/loop2 free:0.0GB | total:0.0GB"
    "msg": "Device /dev/loop4 free:0.0GB | total:0.0GB"
```
