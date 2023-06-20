# Ubuntu / Debian Repository

This is the repository that I use for publishing application packages.

List of current [packages](PACKAGES.md) in the repositories.

## Ubuntu

| version | name   |
|---------|--------|
| 22.04   | jammy  |
| 20.04   | focal  |
| 18.04   | bionic |
| 16.04   | xenial |
| 14.04   | trusty |

## Debian

|version|name|
|------|------|
|12|bookworm|
|11|bullseye|
|10|buster|
|9|stretch|
|8|jessie|

## Setup Repository

### Debian 12 bookworm

    sudo apt install apt-transport-https
    sudo curl -sS -fsSLo /usr/share/keyrings/adelolmo-archive-keyring.gpg https://adelolmo.github.io/andoni.delolmo@gmail.com.gpg
    echo "deb [signed-by=/usr/share/keyrings/adelolmo-archive-keyring.gpg] https://adelolmo.github.io/$(lsb_release -cs) $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/adelolmo.github.io.list

### For older versions

    sudo apt-get install apt-transport-https
    wget -O - http://adelolmo.github.io/andoni.delolmo@gmail.com.gpg.key | sudo apt-key add -
    echo "deb http://adelolmo.github.io/$(lsb_release -cs) $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/adelolmo.github.io.list
