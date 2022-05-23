# Open Cravat BIBBOX application

This container can be installed as [BIBBOX APP](https://bibbox.readthedocs.io/en/latest/ "BIBBOX") or standalone.
 
After the installation follow these [instructions](INSTALL-APP.md)

## Hints
* initial user/password: **admin / admin**

## Install within BIBBOX

Within BIBBOX you can use the [BIBBOX](https://bibbox.readthedocs.io/en/latest/ "BIBBOX") to install a lot of software tools. After the installation is finished you can start your application in the dashboard.

## Docker Images Used
 * [karchinlab/opencravat](https://hub.docker.com/r/karchinlab/opencravat), offical open-cravat-frontend container 
 
## Standalone Installation

To install the app locally execute the commands:
* Clone the git repository: 
  * `git clone https://github.com/bibbox/app-open-cravat`
* Change the current directory to app-open-cravat: 
  * `cd app-open-cravat/` 
* Create the docker network `bibbox-default-network`: 
  * `docker network create bibbox-default-network`
* Run **docker-compose up** in the root folder of the project: 
  * `docker-compose up -d`
* **Alternatively** on a *Linux* system run the bash script `intsall.sh` after cloning and change the working directory to the git repository directory.
 

After the installation (might take a few minutes) open **http://localhost:8080** in your browser to access Open Cravat.
The default admin login is **user:admin/pw:admin**, this can be changed in `docker-compose.yml`.

## Mounted Volumes
* ./data/path/

