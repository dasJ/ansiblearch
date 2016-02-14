# Letsencrypt

This role installs letsencrypt with a systemd timer unit and creates a configuration file with webroot or standalone authenticator. It will automatically generate a new certificate when the configuration changes.

## Variables

### Required
- `letsencrypt_email` - Admin email address
- `letsencrypt_domains` - Array of the domains the certificate will be issued for

### Optional
- `letsencrypt_key_size` - Size of the key (defaults to 4096)
- `letsencrypt_authenticator` - Either `webroot` or `standalone` (defaults to `webroot`)
- `letsencrypt_webroot_path` - Path for webroot authenticator (defaults to /tmp/letsencrypt-auto)
- `letsencrypt_standalone_challenge` - Challenge for standalone authentication, either `tls-sni-01` or `http-01` (defaults to `tls-sni-01`)
- `letsencrypt_noregen` - Set to anything to prevent certificate regeneration on configuration change.
