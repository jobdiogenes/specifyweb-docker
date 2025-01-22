# [Specify 7](https://www.specifysoftware.org/products/specify-7/) (WEB) Docker 
Specify WEB (7+) Software - docker compose scripts

These are docker files and scripts develop to deploy Specify7.

^ These are __not__ full production scripts because:
- need backup scripts
- need use _docker secrets_ instead ___.env__ 
- need _swarm_ kubernets like scripts and adjustmet 

## Main features

- Alpine based image (small than default)
- Easy understand
- Persistent Volumes and Network
- __SAFE__: UI and REST API behind NGINX
- __SAFE__: Migrate only when build
- __services__:
```
1. mariadb
2. asset-server
3. report-runner
4. specify7
5. nginx
```
- Script __build.sh__ ro build all services

## How to use

- requeriments: (Linux, Docker)

```bash
git clone https://github.com/jobdiogenes/specifyweb-docker
cd specify-webdocker
sh build.sh
```
