
# Install the bzflag ansible role

```bash
# Create a directory for the ansible role. 
install -d ~/.ansible/roles/computate.computate_ansible

# Clone the bzflag ansible role. 
git clone git@github.com:computate-org/computate_ansible.git ~/.ansible/roles/computate.computate_ansible
cd ~/.ansible/roles/computate.computate_ansible
```

# Update the submodules to load all of the child Ansible roles. 

```bash
git submodule update --init --recursive
```

# Run the individual playbooks to install the applications locally. 

```bash
ansible-playbook install_bzflag.yml
ansible-playbook install_mari0.yml
ansible-playbook install_supertuxkart.yml
```

# Add new child roles. 

You can add new child roles like this: 

```bash
git submodule add https://github.com/computate-org/computate_sqlite.git roles/computate.computate_sqlite
```
