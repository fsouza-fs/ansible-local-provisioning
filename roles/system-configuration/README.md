# System Configuration Role

This role ensures that the necessary system packages are installed and that the APT package list is updated and upgraded.

## Tasks

- Update and upgrade APT packages.
- Install essential system packages like curl, git, wget, gnupg2, etc.

## Dependencies

No Dependencies are required for this role.

## Variables

- `local_user`: The local user to which some configurations will be applied.

## Example Playbook

```yaml
- hosts: all
  roles:
    - system-configuration
