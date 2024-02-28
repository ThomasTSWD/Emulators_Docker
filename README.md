# Emu ANDROID

## Image

https://github.com/budtmo/docker-android

## Stopper arreter containers

> docker stop $(docker ps -a -q)

> docker rm $(docker ps -a -q)

## Lancer image du cher butmo

> docker run -d -p 6080:6080 -e EMULATOR_DEVICE="Samsung Galaxy S10" -e WEB_VNC=true --device /dev/kvm --name android-container budtmo/docker-android:emulator_11.0

http://localhost:6080

## SERT A RIEN MAIS BON

Aller dans la console Android 

> docker exec -it bf70e1d47424 bash

Dans la console android

> emulator -list-avds

> emulator -avd samsung_galaxy_s10_11.0

# SAFARI

> docker run --rm -it --shm-size=3g -p 7900:7900 -p 4444:4444 -p 5900:5900 -e ARCH='aarch64' jamesmortensen/webkitwebdriver-epiphany:latest

mdp : secret

Terminal dans noVnc > epiphany

Enjoy !

# RAPPELS DOCKER

Voir tous les containers

Docker ps -a
