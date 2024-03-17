### Automated Deployment of Dockerized Apache with Ansible

This repository contains an Ansible playbook designed to automate the deployment of an Apache Docker container and configure its networking. The playbook streamlines the deployment process, ensuring consistency and efficiency in deploying containerized applications.

### Control Machine Setup (WSL):

To set up WSL (Windows Subsystem for Linux) on the control machine and install Ansible:

1. Enable WSL feature using Powershell in admin mode:
    ```powershell
    wsl --install
    ```
2. Install Ansible:
    ```bash
    sudo apt update
    sudo apt install ansible
    ```

### Virtual Machine Setup:

1. Set up virtualization software (e.g., VirtualBox or VMware).
2. Download the Ubuntu ISO file from the official Ubuntu website.
3. Launch the virtualization program and create a new virtual machine.
4. Install Ubuntu on the virtual system using the downloaded ISO file.

### Open SSH:

Install and run SSH in both the control and target machines:
```bash
sudo apt update
sudo apt install openssh-server
sudo service ssh start
```

### Ansible Playbook Execution:
To deploy the Dockerized Apache container using the provided Ansible playbook:

1. Clone this repository:
```bash
git clone https://github.com/TijuThampan/Network_Assignment.git
```

2. Run the Ansible playbook:
```bash
sudo ansible-playbook deploy_docker.yml
```

3. Verify the successful deployment and accessibility of the Apache service.


