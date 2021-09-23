```yaml
[root@localhost Netbox]# ansible-playbook netbox-uri.yml 

PLAY [Get site data] ******************************************************************************************************************************************************************

TASK [Gathering Facts] ****************************************************************************************************************************************************************
ok: [localhost]

TASK [Find device in Netbox] **********************************************************************************************************************************************************
ok: [localhost]

TASK [debug] **************************************************************************************************************************************************************************
ok: [localhost] => {
    "_output": {
        "allow": "GET, POST, PUT, PATCH, DELETE, HEAD, OPTIONS",
        "api_version": "2.11",
        "changed": false,
        "connection": "close",
        "content_length": "1202",
        "content_type": "application/json",
        "cookies": {},
        "cookies_string": "",
        "date": "Thu, 23 Sep 2021 13:28:15 GMT",
        "elapsed": 0,
        "failed": false,
        "json": {
            "count": 1,
            "next": null,
            "previous": null,
            "results": [
                {
                    "asset_tag": null,
                    "cluster": null,
                    "comments": "added by Ansible",
                    "config_context": {},
                    "created": "2021-05-29",
                    "custom_fields": {},
                    "device_role": {
                        "display": "Router",
                        "id": 1,
                        "name": "Router",
                        "slug": "router",
                        "url": "http://192.168.1.192:8000/api/dcim/device-roles/1/"
                    },
                    "device_type": {
                        "display": "iosv",
                        "display_name": "Cisco iosv",
                        "id": 1,
                        "manufacturer": {
                            "display": "Cisco",
                            "id": 1,
                            "name": "Cisco",
                            "slug": "cisco",
                            "url": "http://192.168.1.192:8000/api/dcim/manufacturers/1/"
                        },
                        "model": "iosv",
                        "slug": "iosv",
                        "url": "http://192.168.1.192:8000/api/dcim/device-types/1/"
                    },
                    "display": "R6",
                    "display_name": "R6",
                    "face": null,
                    "id": 8,
                    "last_updated": "2021-05-29T14:05:14.350357Z",
                    "local_context_data": null,
                    "location": null,
                    "name": "R6",
                    "parent_device": null,
                    "platform": null,
                    "position": null,
                    "primary_ip": null,
                    "primary_ip4": null,
                    "primary_ip6": null,
                    "rack": null,
                    "serial": "9ONMNHBN5VR868MHTXDZM",
                    "site": {
                        "display": "Home",
                        "id": 1,
                        "name": "Home",
                        "slug": "home",
                        "url": "http://192.168.1.192:8000/api/dcim/sites/1/"
                    },
                    "status": {
                        "label": "Active",
                        "value": "active"
                    },
                    "tags": [],
                    "tenant": null,
                    "url": "http://192.168.1.192:8000/api/dcim/devices/8/",
                    "vc_position": null,
                    "vc_priority": null,
                    "virtual_chassis": null
                }
            ]
        },
        "msg": "OK (1202 bytes)",
        "redirected": true,
        "referrer_policy": "same-origin",
        "server": "Unit/1.22.0",
        "status": 200,
        "url": "http://192.168.1.192:8000/api/dcim/devices/?name=R6",
        "vary": "Accept, Cookie, Origin",
        "x_content_type_options": "nosniff",
        "x_frame_options": "SAMEORIGIN"
    }
}

PLAY RECAP ****************************************************************************************************************************************************************************
localhost                  : ok=3    changed=0    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0   

[root@localhost Netbox]# 
```
