# Ansible Role: Apache HTTPd 2.x
![Build Status](https://travis-ci.org/jhu-sheridan-libraries/ansible-role-httpd.svg?branch=master)

## Requirements:
For SSL/TLS you will need to supply your own certificates.  This can be done via variable:
``` yaml
ssl_certs:
  host.domain.tld:
    cert: |
      -----BEGIN CERTFICATE-----
      Masasdfklasdjflka12312j1lk12j3kl1hjk4hlkj3h4
      -----END CERTIFICATE-----
    interm: |
      -----BEGIN CERTIFICATE-----
      Many characters go here
      -----END CERTIFICATE-----
    key: |
      -----BEGIN RSA PRIVATE KEY-----
      EVEN MORE CHARACTERS...
      -----END RSA PRIVATE KEY-----
```

## Role Variables:
Default variables and examples can be found in 'defaults/main.yml':

    apache_httpd_version: latest

This will allow you to lock apache into a specific version and keep the role from running the latest version.  
