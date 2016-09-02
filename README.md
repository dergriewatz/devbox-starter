# Symfony Starter Vagrantbox

This is a minimal Vagrantsetup for running symfony.

```bash
git clone git@github.com:sensiolabs-de/devbox-starter.git
cd devbox-starter
cp config.yml.dist config.yml
nano config.yml
vagrant up
```

## Whats included:

- Ubuntu 16.04 (Xenial Xerus)
- PHP 7
- Apache2 as server
- MySQL (user: `dev`, password: `dev`)
- Provisioning via Ansible
- xdebug script for debugging on command line (preconfigured for PhpStorm)

## Maintainer

Lukas Sadzik (lukas.sadzik@sensiolabs.de)
