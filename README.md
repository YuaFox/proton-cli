# Proton-CLI

Proton-CLI is a custom distribution of [Proton](https://github.com/ValveSoftware/Proton)

## Features
- Run .exe using double click
- Track installed programs: After installing a program you will be able to run it using your launcher.

## Install

### Debian

You can install proton-cli using apt
```
echo "deb [arch=amd64] https://deb.yua.sh stable main" | sudo tee /etc/apt/sources.list.d/yua.list
curl -sS https://deb.yua.sh/pgp-key.public | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/yua.gpg
sudo apt update
sudo apt install proton-cli
```

To be able to run .exes clicking use the following command

```
xdg-mime default proton.desktop application/x-ms-dos-executable
```