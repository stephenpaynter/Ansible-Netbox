## netbox-create-site.yml

 This playbook stands up a site within Netbox which is used to house network devices.

```yaml
[root@localhost Netbox]# ansible-playbook netbox-create-site.yml

PLAY [Standup Site Within Netbox] *****************************************************************************************************************************************************

TASK [Gathering Facts] ****************************************************************************************************************************************************************
ok: [localhost]

TASK [Create site within Netbox with only required information] ***********************************************************************************************************************
ok: [localhost]

PLAY RECAP ****************************************************************************************************************************************************************************
localhost                  : ok=2    changed=0    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0   

[root@localhost Netbox]# 
```
