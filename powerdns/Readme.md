# Powerdns

This role installs and configures a PowerDNS server with a PostgreSQL backend.
It can not configure every option in the configuration file because I am lazy.

## Variables

### Required
- `powerdns_dbhost` - Hostname of the PostgreSQL server
- `powerdns_db` - Name of the PostgreSQL database
- `powerdns_dbuser` - Username of the PostgreSQL database
- `powerdns_dbpassword` - Password of the PostgreSQL database

### Optional
- `powerdns_axfr_ips` - Allow AXFRs from these comma-separated IPs
- `powerdns_dnsupdate_from` - Allow DNS Updates from these comma-separated IPs
- `powerdns_allow_notify_from` - Allow DNS Notifys from these comma-separated IPs
- `powerdns_allow_recursion` - Allow recursion from these comma-separated IPs
- `powerdns_also_notify` - Also notify these comma-separated IPs
