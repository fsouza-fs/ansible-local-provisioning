# Web Browser Installation Role

This role handles the installation of Google Chrome web browser.

## Tasks

- Installs Google Chrome from the official DEB package.

## Dependencies

- system-configuration

## Variables

No variables are needed for this role.

## Example Playbook

```yaml
- hosts: all
  roles:
    - web-browser
