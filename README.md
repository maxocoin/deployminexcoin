# deployminexcoin
Ansible scripts that deploys the Minexcoin wallet and the mininer on a fleshly installed Ubuntu 16.04 machine

First you have to install git with

```
sudo apt-get update
sudo apt-get install git tmux zip
```

Then check out the project with the command

`git clone https://github.com/maxocoin/deployminexcoin.git`
 
And move into it
`cd deployminexcoin` 
 

Install ansible with  `deployminexcoin/system_setup.sh`  or:
```
 sudo apt-get update
 sudo apt-get install software-properties-common
 sudo apt-add-repository ppa:ansible/ansible
 sudo apt-get update
 sudo apt-get install ansible
```


For install the miner, change the `mining_address variable`  in the file `defaults/main.yml`
and type: 
   
`   ansible-playbook -i hosts installMxMiner.yml`


For install the Minex Coin Core wallet, run the ansible script

`  ansible-playbook -i hosts installMinexcoin.yml`
  
 
