# Unifi Ansible Toolbox

## Introduction

Actually the API is only available to display informations of your Unifi devices.
You will find here many playbooks based on my unofficial ansible module using the official API of Unifi : [see more here](https://github.com/erwanclx/UnifiAnsibleModule)

I use many of this which Discord webhook integration to receive notification and it is implemented to be run daily, these playbooks are sample, you can freely edit them to remove discord webhook build 😊

## Configuration

- secrets.yml
*The file will contain your configuration*
```
unifi_api_key: "your_api_key" # STRING (required)
udm_id: "12345678abc" # STRING (optional, only use if you want to use host_status.yml with specific ID)
discord_webhook_url: "https://discord.com/XXXXXXX" # STRING (optional, only use if you want to use Discord notifications)
```

## Playbooks 
- hosts.yml : List your hosts
- host_status.yml : Get update status of Unifi device by ID
- hosts_status.yml : Get update status of all Unifi **devices**
