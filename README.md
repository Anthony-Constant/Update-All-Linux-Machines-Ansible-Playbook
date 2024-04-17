# Ansible Playbook: Update All Linux Machines

## Introduction
This Ansible playbook automates the task of updating package caches on multiple Linux machines within your environment. It ensures that the package cache is refreshed to the latest available versions, thereby aiding in system maintenance and security.

## How It Works
This playbook is written in YAML and utilizes Ansible, an open-source automation tool. It connects to specified hosts and performs the following tasks:
1. Connects to each host using specified credentials.
2. Updates the package cache to fetch the latest available versions of all packages.

## Features
- **Automation**: Eliminates the manual process of updating package caches on multiple Linux machines.
- **Consistency**: Ensures all machines are updated consistently to the latest package versions.
- **Security**: Utilizes secure methods for authentication and privilege escalation.
- **Customization**: Easily adaptable to include additional tasks or customize as needed.

## Getting Started
To use this Ansible playbook, follow these steps:

1. **Prerequisites**:
   - Ensure Ansible is installed on your control machine.
   - Have SSH access to all target Linux machines.
   - Replace `password` in the playbook variables with your sudo password.

2. **Clone the Repository**:
   ```bash
   git clone <repository_url>
   cd <repository_directory>
   
3. **Update Inventory File**:
Edit the `hosts` file to include the IP addresses or hostnames of your target Linux machines.

4. **Run the Playbook**:
   ```bash
    ansible-playbook -i hosts update_linux.yml

5. **Provide Sudo Password**:
Ansible will prompt you to provide the sudo password for privilege escalation.

6. **Verify Updates**:
Once the playbook execution completes, verify that the package caches are updated on all target machines.

7. **Customization (Optional)**:
Modify the playbook (update_linux.yml) to include additional tasks or customize according to your requirements.

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

## Acknowledgements

This script was created by [Anthony Constant](https://anthonyconstant.co.uk/).

## Support My Work

If you like this repository or have used any of the code, please consider showing your support:

- Give it a star ⭐️ to acknowledge its value.
- You can also support me by [buying me a coffee ☕️](https://ko-fi.com/W7W144CAO).
