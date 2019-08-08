## Ubuntu / Debian Repository

This is the repository that I use for publishing application packages.

List of current [packages](PACKAGES.md) in the repositories.

### Setup Repository

Current supported distributions are:

- Ubuntu
    - bionic
    - xenial
    - trusty
- Debian
    - stretch
    - jessie

```markdown
sudo apt-get install apt-transport-https
```

```
wget -O - http://adelolmo.github.io/andoni.delolmo@gmail.com.gpg.key | sudo apt-key add -
echo "deb http://adelolmo.github.io/$(lsb_release -cs) $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/adelolmo.github.io.list
```