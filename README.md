# vnios_ztp_vmware
Zero touch deployment of Infoblox Grid on Vmware vsphere using Ansible

Please download vnios_ztp_vmware.yaml and nios_details.ini files and place them in the same directory. 
nios_details.ini is feeder file for the vnios_ztp_vmware.yaml file. vnios_ztp_vmware.yaml file refers to nios_details.ini for details like grid master fqdn, members fqdn lan1 ip, netmask, gateway grid name, user id , password and shared secret

Under resources section of nios_details.in file please enter ram in MB. Make sure that entered ram translates to an interger value in GB. For example, 2048MB ram translates to 2GB.

Pre-requisites:: 
Ansible server must have pyvmomi and python-infoblox client installed. 

Tested on Ansible 2.8 and vsphere 6.5
For any queries/clarification feel free to send an email to asahu@infoblox.com
