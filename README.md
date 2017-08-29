# Simple Environment Provisioning Solution




This is a complete solution to dynamically launch full environment for mytinytodo app. This project accomplishes the following tasks fully automated.

  - Launch server in aws
  - Configure newly launched server
  - Deploy code to the server
  - Manage webserver
  - Destroy the whole environement after use.

### Prerequisites

  - A linux or unix based host computer
  - Ansible installed
  - AWS account with full privilages on ec2
  - ACCESSKEY and SECRETKEY should be placed in the file ''terrraform_code/.creds''



# Usage
```sh
sh provision.sh --option
```
##### options:

```sh 
--destroy    : Destroys the infrastructure built by the tool
--deployonly : Only does the deployment part of the project
```


### Tech

This provisioning tool uses the following technologies:

* [terraform] - Terraform enables you to safely and predictably create, change, and improve production infrastructure
* [Ansible] - Ansible is the simplest way to automate apps and IT infrastructure. Application Deployment + Configuration Management + Continuous Delivery.

###### NOTE: mysql password is in database playbook. right now there is only root user. 
 username: root
 password: strongpassword
  
   [ansible]: <https://www.ansible.com/>
   [terraform]: <https://www.terraform.io/>
 