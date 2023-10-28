# Development Tools Role

This role sets up various development tools including Node.js, Yarn, VSCode, Docker, Podman, Postman, and configures Git.

## Tasks

- Setup Node.js along with NodeSource repository.
- Install Yarn globally using npm.
- Setup Visual Studio Code along with its repository and GPG key.
- Setup Docker and add the specified user to the docker group.
- Setup Podman along with its repository and GPG key.
- Setup Postman and create a desktop entry for it.
- Configure global Git username and email.

## Dependencies

- system-configuration

## Variables

- `local_user`: The local user to which some configurations will be applied.
- `git_username`: The global Git username.
- `git_email`: The global Git email.

## Example Playbook

```yaml
- hosts: all
  roles:
    - development-tools
