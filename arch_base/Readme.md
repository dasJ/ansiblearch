# Arch base

This role is supposed to build Arch Linux from scratch.
It consists of a script (`initserver`) and the role.

The script is run in the archiso and prepares everything for Ansible.
After running it, reboot and you can use Ansible with this role.
Be sure to check the first few lines of the script, they configuration.

It sets up locales, keymap, hostname, creates users, and more.
It's what every Arch looks like that I install.

The playbook will create netctl configs which start DHCP on every interface.
Your user password will be stored in user-password.txt on your control machine.
Root won't have any password.

## Variables

### Required
- `arch_base_hostname` - Hostname of the system
- `arch_base_fqdn` - FQDN of the system
- `arch_base_username` - Username of the user to be created

### Optional
- `arch_base_locale` - Locale (default: `en_US.UTF-8`)
- `arch_base_collate` - LC_COLLATE value (default: `C`)
- `arch_base_keymap` - Keymap for physical logon (default: `de-latin1-nodeadkeys`)
- `arch_base_timezone` - Timezone of the system, relative to `/usr/share/zoneinfo` (default: `Europe/Berlin`)
- `arch_base_locales` - Array with locales to be generated (default: all `de_DE` and `en_US`)
