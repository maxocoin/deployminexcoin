# deployminexcoin
Ansible scripts that deploys the Minexcoin wallet on fleshly installet Ubuntu 16.04 machine

First you have to install git with

sudo apt-get install git


Then check out the proyect with the command
git clone https://github.com/maxocoin/deployminexcoin.git


Install ansible with

 sudo apt-get update
 sudo apt-get install software-properties-common
 sudo apt-add-repository ppa:ansible/ansible
 sudo apt-get update
 sudo apt-get install ansible


For install the Minex Coin Core wallet, run the ansible script

  ansible-playbook -i hosts installMinexcoin.yml
  
 
For install the miner, change the mining_address variable  in the file defaults/main.yml
and type 
   
   ansible-playbook -i hosts installMxMiner.yml

