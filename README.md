# README.md
# Ansible Role: mats116.papertrail

An Ansible role that configure rsyslog for **[papertrail](https://papertrailapp.com/)** on **Ubuntu 14.04 LTS**

Use TLS orver TCP.

## Requirements

- rsyslog

## Role Variables

Available variables are listed below, along with default values:

papertrail_host:
papertrail_port:
papertrail_syslog_facility: local7

## Dependencies

none

## Example Playbook

    - hosts: web-server
      roles:
        - role: mats116.papertrail
          papertrail_host: log2
          papertrail_port: 29731
          papertrail_syslog_facility: local3

## License

MIT
