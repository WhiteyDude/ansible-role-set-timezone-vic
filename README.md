# Set timezone to Australia/Melbourne

Pretty basic, restarts rsyslog to ensure log timestamps are up to date, no restart required. Could easily be adapted to use variables and be smarter, but suits my needs.

## Example

```
---
- hosts: all
  become: yes
  roles:
    - {role: ./roles/ansible-role-set-timezone-vic}
```