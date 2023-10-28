# Security Configuration Role

This role aims to fortify the security posture of the Ubuntu machine by configuring the UFW firewall, enabling automatic security updates, setting correct permissions on sensitive files, and installing AppArmor.

## Tasks

- Ensure UFW is installed.
- Deny all incoming traffic by default.
- Allow all outgoing traffic by default.
- Deny incoming SSH.
- Allow established connections to remain active.
- Enable UFW.
- Ensure unattended-upgrades is installed.
- Enable automatic security updates.
- Set correct permissions on sensitive files.
- Ensure AppArmor is installed.

## Dependencies

- system-configuration

## Variables

No variables are needed for this role.

## Example Playbook

```yaml
- hosts: all
  roles:
    - security-configuration
