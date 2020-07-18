## Automated ELK Stack Deployment

The files in this repository were used to configure the network depicted below.

![Image of VMs](https://github.com/BradwanTV/UoUElkStackProject/blob/master/Images/Project%20Complete.jpg)

These files have been tested and used to generate a live ELK deployment on Azure. They can be used to either recreate the entire deployment pictured above. Alternatively, select portions of the playbook files may be used to install only certain pieces of it, such as Filebeat.

Playbook Files Can be found Below
https://github.com/BradwanTV/UoUElkStackProject/tree/master/Files/Ansible%20Playbook%20Files

This document contains the following details:
- Description of the Topologu
- Access Policies
- ELK Configuration
  - Beats in Use
  - Machines Being Monitored
- How to Use the Ansible Build


### Description of the Topology

The main purpose of this network is to expose a load-balanced and monitored instance of DVWA, the D*mn Vulnerable Web Application.

Load balancing ensures that the application will be highly stable, in addition to restricting unauthorized users to the network.

Integrating an ELK server allows users to easily monitor the vulnerable VMs for changes to the log fiels and system metrics.

The configuration details of each machine may be found below.
_Note: Use the [Markdown Table Generator](http://www.tablesgenerator.com/markdown_tables) to add/remove values from the table_.

| Name      | Function | IP Address | Operating System |
|-----------|----------|------------|------------------|
| Jump Box  | Gateway  | 10.0.0.4   | Linux            |
| web-01    | Webserver| 10.0.0.5   | Linux            |
| web-02    | Webserver| 10.0.0.6   | Linux            |
| web-03    | Webserver| 10.0.0.7   | Linux            |
| ELK-Server| Webserver| 10.1.0.4   | Linux            |

### Access Policies

The machines on the internal network are not exposed to the public Internet. 

Only the Jumpbox machine can accept connections from the Internet. Access to this machine is only allowed from the following IP addresses:
HomeIP - Removed for privacy reasons

Machines within the network can only be accessed by Jumpbox.

A summary of the access policies in place can be found in the table below.

### Elk Configuration

Ansible was used to automate configuration of the ELK machine. No configuration was performed manually, which is advantageous as we are able to scale to any size of needed webservers and are able to redeploy within minutes if servers go down.

The playbooks implements the following tasks:
- _TODO: In 3-5 bullets, explain the steps of the ELK installation play. E.g., install Docker; download image; etc._
- ...
- ...

The following screenshot displays the result of running `docker ps` after successfully configuring the ELK instance.

![TODO: Update the path with the name of your screenshot of docker ps output](Images/docker_ps_output.png)

### Target Machines & Beats
This ELK server is configured to monitor the following machines, along with FileBeat & MetricBeat

| Name      | Function | IP Address | Operating System |
|-----------|----------|------------|------------------|
| web-01    | Webserver| 10.0.0.5   | Linux            |
| web-02    | Webserver| 10.0.0.6   | Linux            |
| web-03    | Webserver| 10.0.0.7   | Linux            |

These Beats allow us to collect the following information from each machine:

### Using the Playbook
In order to use the playbook, you will need to have an Ansible control node already configured. Assuming you have such a control node provisioned: 

SSH into the control node and follow the steps below:
- Copy the _____ file to _____.
- Update the hosts file to your webservers IP address
- Run the playbook, and navigate to ____ to check that the installation worked as expected.

_TODO: Answer the following questions to fill in the blanks:_
- _Which file is the playbook? Where do you copy it?_
- _Which file do you update to make Ansible run the playbook on a specific machine? How do I specify which machine to install the ELK server on versus which to install Filebeat on?_
- _Which URL do you navigate to in order to check that the ELK server is running?

_As a **Bonus**, provide the specific commands the user will need to run to download the playbook, update the files, etc._
