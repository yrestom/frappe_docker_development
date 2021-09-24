# frappe_docker_development for bloomstack
This will create 3 container for development{frappe,mariadb,redis}
frappe container contains all the bench depedencies + ohmyzsh + git + nodejs
## supported systems
- ubuntu >18.04 (x86_64, arm64)
- MacOs (x86_64, M1 chips)

##  Prerequisites<h2 >
* docker
* vscode (with [remote-container](https://github.com/Microsoft/vscode-remote-release) extension)

##  How to Start<h2 >
* ``` git clone https://github.com/sahilk25/frappe_docker_development.git```
* ``` cd frappe_docker_development && mkdir development```
* ``` docker build -t bench:latest bench_docker```
* open vscode in current directory(code .)

* click on reopen in container
## Custom commands
* ```bs``` #it will close all process running on bench port and start the bench
* ```gs``` #it will edit the .git/conf file so we can fetch all branches in app
## What it will create
* frappe-bench directory in development directory
* get-app frappe erpnext bloomstack_core from bloomstack repo
* set up some bench commands{check [setupbench.sh](https://github.com/sahilk25/frappe_docker_development/blob/main/bench_docker/setupbench.sh) in bench_docker directory}
#### Thnx to frappe_docker
https://github.com/frappe/frappe_docker click for more information

