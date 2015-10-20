# ansible-role-papertrail
Ubuntu 14.04 LTS

## Synopsis

Adds rsyslog config for [papertrail](https://papertrailapp.com/).
Use TLS orver TCP.

## Requirements

- rsyslog

## Variables

| parameter | required | default | choices | comments |
| --- | --- | --- | --- | --- |
| papertrail_host | yes |  |  |  |
| papertrail_port | yes |  |  |  |
| papertrail_syslog_facility | yes | local7 |  |  |

## Examples

```yaml:paybook.yaml
- hosts: all
  sudo: yes
  roles:
    - role: papertrail
      papertrail_host: log2
      papertrail_port: 29731
      papertrail_syslog_facility: local3
```
