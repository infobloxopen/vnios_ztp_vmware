# vnios_ztp_vmware
Zero touch deployment of Infoblox Grid on Vmware vsphere using Ansible

## For standalone grid master deployment
Please download vnios_ztp_vmware.yaml and nios_details.ini files and place them in the same directory. 
nios_details.ini is feeder file for the vnios_ztp_vmware.yaml file. vnios_ztp_vmware.yaml file refers to nios_details.ini for details like grid master fqdn, members fqdn lan1 ip, netmask, gateway grid name, user id , password and shared secret

Under resources section of nios_details.in file please enter ram in MB. Make sure that entered ram translates to an interger value in GB. For example, 2048MB ram translates to 2GB.

## For HA grid master deployment
Download vnios_ztp_HA_vmware.yaml and nios_details_HA.ini files and place them in the same directory. 
nios_details_HA.ini is feeder file for the vnios_ztp_HA_vmware.yaml file. vnios_ztp_HA_vmware.yaml file refers to nios_details_HA.ini for details like grid master fqdn, lan1 ip, netmask, gateway, HA_vip, grid name, user id , password and shared secret.

Under resources section of nios_details_HA.in file please enter ram in MB. Make sure that entered ram translates to an interger value in GB. For example, 2048MB ram translates to 2GB.

## Pre-requisites:: 
Ansible server must have pyvmomi and python-infoblox client installed. 

Tested on Ansible:2.8.5, pyvmomi:6.7.1, infoblox-client:0.4.23 and vsphere 6.5

For any queries/clarifications feel free to send an email to kvasudevan@infoblox.com

Youtube video --> https://www.youtube.com/watch?v=OmLZF763C34
