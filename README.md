# Unatended Installation

## Prerequisites
git
ansible

## ansiurl='https://github.com/jschulthess/ansible-pull-update.git' # URL of the playbook repository
branch/tag/commit to checkout
```bash
checkout='develop'                                            
```
directory to checkout repository to
```bash
directory='/var/projects/ansible-pull-update'           
```
where to put the logs
```bash
logfile='/var/log/ansible-pull-update.log'                            
```

sudo ansible-pull -o -C ${checkout} -d ${directory} -i ${directory}/inventory -U ${url} 2>&1 | sudo tee -a ${logfile}ble pull



### this and that
ansible-galaxy install gantsign.oh-my-zsh
nansible-playbook playbook.yml -i hosts -e action=install

# TODOS
+ fzf does not work
+ install lg
```
sudo add-apt-repository ppa:lazygit-team/release
sudo apt-get update
sudo apt-get install lazygit
install vim
```
