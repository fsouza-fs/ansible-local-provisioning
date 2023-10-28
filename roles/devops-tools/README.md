# DevOps Tooling Role

This role sets up various tools essential for a DevOps Engineer such as AWS CLI, GCloud, Kubectl, Helm, and Terraform.

## Tasks

- Setup AWS CLI v2.
- Setup Google Cloud SDK.
- Setup Kubernetes command-line tool (kubectl).
- Setup Helm, a package manager for Kubernetes.
- Setup Terraform for infrastructure automation.

## Dependencies

- system-configuration

## Variables

- `lsb_release_name`: The codename of the Ubuntu release.

## Example Playbook

```yaml
- hosts: all
  roles:
    - devops-tools
