# Ansible Playbooks Repository

This repository contains Ansible playbooks for automating various tasks on different types of hosts. The playbooks are organized based on host types, and each playbook is tagged for better organization.

## Playbooks

### `ansible_playbook_demo.yml`

- **Description:** Demonstration playbook for setting up Apache2, MariaDB, and Samba on different hosts.
- **Tags:**
  - `apache2`: Configures and starts the Apache2 service.
  - `mariadb`: Installs MariaDB server.
  - `samba`: Installs Samba on Ubuntu.
  - `user`: Adds a new user with SSH key and sudoers configuration.
  - `sudoers`: Configures sudoers file for the added user.
  - `timeout`: Modifies Apache2 timeout on Ubuntu.
  - `ubuntu`: Tasks specific to Ubuntu hosts.

## Hosts

- **`web01`**: Host for web services (Apache2 setup).
- **`db01`**: Host for database services (MariaDB setup).
- **`file01`**: Host for file sharing services (Samba setup).
- **`all`**: General tasks applicable to all hosts.

## Usage

1. Ensure Ansible is installed on the control machine.
2. Update the inventory file (`inventory`) with your host information.
3. Run the desired playbook using the following command:

   ```bash
   ansible-playbook -i inventory <playbook_name>.yml
  ```

## License

This repo is made available under the MIT license

