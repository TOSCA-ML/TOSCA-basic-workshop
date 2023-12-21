# TOSCA-basic-workshop

## Environment
Two VMs
1. TOSCA-main 	172.17.91.243
2. TOSCA-target  172.17.91.195

## S1. Installation of xOpera

xOpera is distributed as a Python package that is regularly published on PyPI. So the simplest way to test opera is to install it into a virtual environment. 

* Login to ```TOSCA-main``` VM
* Update ubuntu: ```sudo apt update```
* Create and change directory to a new opera directory: ```mkdir $HOME/opera && cd $HOME/opera```
* Install python virtual environment if not present ```sudo apt install python3-venv python3-wheel python-wheel-common```
* Create a virtual environment: ```python3 -m venv .venv```
* Activate the virtual environment:  ```. .venv/bin/activate```
* Install pip : ```pip install pip==21.3.1``` 
* Now it is the time to install opera: ```pip install opera==0.6.8```
* If you receive some errors or warnings related to ```pyyaml``` versions, please ignore them.
* Check the installation by only issuing opera command
![Opera Version](img/Opera_version.jpeg)

#### _Note_: 
Remember that opera requires python 3 and a virtual environment. Before you issue any opera command, make sure that you have activated the virtual environment.
```
cd $HOME/opera
. .venv/bin/activate
opera
```
## S2. Get the TOSCA definitions
* Login to ```TOSCA-main``` VM
* Make sure you have activated the virtual environment.
* cd $HOME
* Fork https://gitlab.cs.ut.ee/devops22fallpub/radon-particles repository ```git clone https://gitlab.cs.ut.ee/devops22fallpub/radon-particles```



## References :
- xOpera Github repo: https://github.com/xlab-si/xopera-opera 
- xOpera documentation is available here: https://xlab-si.github.io/xopera-docs/index.html 
- Cli command references: https://xlab-si.github.io/xopera-docs/02-cli.html#cli-commands-reference 
