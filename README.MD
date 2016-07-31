###Install Openstack using ansible

####How to use

- Install requirements

```
Vagrant
Ansible version 2.0.0.1 

```
- Clone this project 

```
git clone https://github.com/greatbn/openstack-ansible-install.git
cd openstack-ansible-install
git checkout virtualbox/mitaka
```

- Create Infras

```
vagrant up
```

- Install Openstack

```
ansible-playbook -i hosts -s site.yml
```

- Have a coffee

- Access Horizon at

```
https://10.30.0.21/horizon
```
