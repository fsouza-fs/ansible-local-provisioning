# Terminal Shell Configuration Role

This role sets up the terminal environment by installing Zsh shell, Oh My Zsh, and the Spaceship theme. It also changes the default terminal font to Fira Code.

## Tasks

- Install Zsh and Oh My Zsh.
- Set up the Spaceship theme for Oh My Zsh.
- Change the default terminal font to Fira Code.

## Dependencies

- system-configuration

## Variables

- `local_user`: The local user to which some configurations will be applied.

## Example Playbook

```yaml
- hosts: all
  roles:
    - terminal-shell-configuration
