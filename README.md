# cloud-init configs for launching OverLogic nodes.
v0.9 - 11/2021 | Maintained by *Nik Ferios/OverLogic*

## Available node types:
- ol_commander (AMD64) - WireGuard, Portainer, Nginx Proxy Manager
- ol_node (AMD64) - Portainer Agent

## Included on all templates:
### node hardening
    - passwordless ssh
    - ufw
    - fail2ban
    - unattended security upgrades
### node user
    - import authorized ssh public keys from github
    - passwordless sudo
    - set temp password
### docker
    - engine
    - compose
    - ipv6
    - log rotation
    - enabled experimental features
    - enabled metrics collection through prometheus
- timezone set to Athens-GR

## Usage:
- Select template
- Edit lines starting with #! appropriately
- Copy amended template as user-data
- Launch instance
