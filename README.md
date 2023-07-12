# repoAppReact
DOCKERIZE A REACT WEB APPLICATION
--####################################################################################
									GIT BASH
--####################################################################################

git config user.name
git config user.email

git config --global user.name "AlvaradoMarcos2090"
git config --global user.email "alvaradomarcos2090@gmail.com"

--####################################################################################
Generar llave LOCAL para GitHub

ssh-keygen -t rsa -b 4096 -C "alvaradomarcos2090@gmail.com"
cat ~/.ssh/id_rsa.pub			<<admin>>

--####################################################################################
Agregar proyecto a GitHub

git init
git add -A
git commit -m "primer commit"
git branch -M main
git remote add origin <<REPO_NAME_SSH git@github.com:<<userName>>/<<repo>>.git>>
git remote -v
git pull --rebase origin main
git push origin main

--####################################################################################
Promover cambios

git add -A
git commit -m "update"
git push origin main

--####################################################################################
Promover branch to master
git push -f origin/main:master 