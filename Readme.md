# Ansible roles for Arch Linux

These are my Ansible roles that I use in many of my Arch playbooks.
This file should provide an overview.

## Setup

These roles are supposed to set up Arch Linux (basic arch, networking, ...)
- `arch_base` - A simple and generic arch
- `serverpower` - Don't accidentally shut down servers
- `netctl_profile` - Generate netctl profiles
- `docker_setup` - Install Docker
- `postgres_setup` - Instal PostgreSQL

System maintenance:
- `powerdns` - Configure a PowerDNS Server with PostgreSQL
- `letsencrypt` - Install letsencrypt and maintain a configuration file
- `nginx`- Install and maintain configuration of nginx
