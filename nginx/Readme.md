# Nginx

This role sets up and configures an nginx server with SSL (with OCSP), letsencrypt webroot support, and status cats.

## Variables

### Required
- `nginx_ssl_certificate` - Path to certificate with attached chain
- `nginx_ssl_key` - Path to the private key
- `nginx_ssl_trusted` - Path to a trusted chain for OCSP
- `nginx_default_webroot` - Path of the default root directory (like `/srv/http/mydomain.tld`)
- `nginx_letsencrypt_webroot_dir` - Path of the webroot directory of letsencrypt

### Optional
- `nginx_upstreams` - Array of upstream objects looking like this: `[ { name: somename, servers: [ "localhost:1234", "localhost:2345 backup" ] } ]`
- `nginx_status_cats_path` - Path where the HTTP status cats should be put (defaults to /srv/http/nginx-status-cats)
