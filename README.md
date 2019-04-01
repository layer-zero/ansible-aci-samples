# ansible-aci-samples
Sample ansible playbooks leveraging the aci-ansible module.

To try them out first generate a key pair using:
```
openssl req -new -newkey rsa:1024 -days 36500 -nodes -x509 -keyout ansible.key -out ansible.crt -subj '/CN=Ansible /O=Layer Zero/C=NL'
```
Then add a hosts file with the following structure:
```
[apic:vars]
username = <your apic username>
password = <your apic password>

[apic]
<your apic fqdn or ip address>
```
