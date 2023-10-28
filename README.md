# Linux Machine Provisioning Playbook

This Ansible playbook is designed to provision a freshly installed Ubuntu 22.04 machine with essential tools, applications, and configurations to make it ready to be used by a developer or DevOps Engineer. Whether you've just formatted your machine or you're setting up a new one, this playbook will automate the setup process for you.

## Features

- Updates and upgrades existing APT packages.
- Applies security configurations
- Installs essential packages like curl, git, wget, and others.
- Genrates an SSH Key
- Configures Git with user name and email.
- Installs Node.js, Yarn, Visual Studio Code, Google Chrome, Docker, AWS CLI, Google Cloud SDK, and others.
- Installs Oh My Zsh, the Spaceship theme, and Zinit for a better terminal experience.
- Sets up Zsh as the default shell.
- And more...

## Prerequisites

- Ubuntu 22.04 machine.
- Ansible installed on the machine.
- Internet connection to download packages and applications.

## Usage

1. Clone this repository to your local machine:
    ```bash
    git clone https://github.com/your-username/linux-provisioning-playbook.git
    cd linux-provisioning-playbook

2. Customize the vars.yml file:  
    The vars.yml file contains variables that are used throughout the playbook. You can customize this file to suit your preferences. For example, you can update the local_user, git_user_name and git_user_email variables to your own user, git username and git email.

    ```yaml
    local_user: "Your user"
    git_user_name: "Your git username"
    git_user_email: "your.git.email@example.com"

3. Run the playbook:  
    The -K flag is used to prompt for the sudo password.

    ```bash
    ansible-playbook -i inventory.ini -K playbook.yml

## Customization
You can further customize the playbook to better suit your needs by modifying the main.yml file directly.

## Contribution
Feel free to fork this repository, make changes, and submit pull requests. Contributions are welcome!

## License
This project is licensed under the MIT License - see the LICENSE.md file for details.
