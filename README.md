# Server Development Playbook
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9e/UbuntuCoF.svg/1024px-UbuntuCoF.svg.png?20120210072525" alt="Ubuntu Logo">
An ansible playbook for setting up ubuntu servers and vms.

<h2>How to use</h2>

<b>1. Install Ansible</b>
To install Ansible,
    do ```sudo apt-get install ansible``` on Ubuntu/Debian
    or ```brew install ansible``` on macOS using <a href="https://brew.sh">Homebrew</a>

<b>2. Clone git repository</b>
To clone the repo,
    goto <a href="https://github.com/tripalc/server-dev-playbook">https://github.com/tripalc/server-dev-playbook</a> and click 'Code', then select 'Download ZIP'
    or, type ```ssh git@github.com:tripalc/server-dev-playbook.git``` into a terminal

<b>3. Edit the configuration file</b>
The configuration file helps you make your Ubuntu machine the way you want it.
To edit the configuration, open the 'config.yml' file inside of nano, vim, VS Code, or Notepad!

<b>4. Edit the inventory file</b>
The inventory file tells Ansible what machines to login to and execute the playbook on.
To edit the inventory, open the 'inventory.ini' file inside of nano, vim, VS Code, or Notepad, and type in the IP Adresses or hostnames of the servers/vms you want to control.

<b>5. Run the playbook</b>
To run the playbook, go into a terminal and type this command:
    ```ansible-playbook ./server-dev.yml -i ./inventory.ini --user [CLIENT USERNAME HERE] --ask-pass --ask-become-pass```
*If you get an error, check you have put the username in the command, you are in the correct directory, you entered both the SSH password and the BECOME password correctly (these are usually the same, and they won't show anything when you type.), and that you have ssh'ed into them at least once on the machine that you are running the playbook from

<b>If there are any other issues, </b><a href="https://github.com/tripalc/server-dev-playbook/issues">Click here.</a>