# Ubuntu / Debian Repository

This is the repository that I use for publishing application packages.

List of current [packages](PACKAGES.md) in the repositories.

> [!IMPORTANT]
> If you are prompt with this message:
> Warning: https://adelolmo.github.io/trixie/dists/trixie/InRelease: Policy will reject signature within a year, see --audit for details

> Please download the signature key again:> 
> sudo curl -sS -fsSLo /usr/share/keyrings/adelolmo-archive-keyring.gpg https://adelolmo.github.io/andoni.delolmo@gmail.com.gpg


## Ubuntu

| version | name   |
|---------|--------|
| 24.04   | noble  |
| 22.04   | jammy  |
| 20.04   | focal  |
| 18.04   | bionic |
| 16.04   | xenial |
| 14.04   | trusty |

## Debian

|version|name|
|------|------|
|13|trixie|
|12|bookworm|
|11|bullseye|
|10|buster|
|9|stretch|
|8|jessie|

## Setup Repository

    sudo apt install apt-transport-https
    sudo curl -sS -fsSLo /usr/share/keyrings/adelolmo-archive-keyring.gpg https://adelolmo.github.io/andoni.delolmo@gmail.com.gpg
    echo "deb [signed-by=/usr/share/keyrings/adelolmo-archive-keyring.gpg] https://adelolmo.github.io/$(lsb_release -cs) $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/adelolmo.github.io.list
