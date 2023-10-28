# Communication Tools Role

This role installs communication tools such as Zoom and Discord on your system.

## Tasks

Here are the main tasks that are performed by this role:

- Install Zoom
- Install Discord

## Dependencies

- system-configuration

## Variables

No variables are needed for this role.

## Example Playbook

```yaml
- hosts: all
  roles:
     - communication-tools
