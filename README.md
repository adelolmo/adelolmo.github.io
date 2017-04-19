## Ubuntu / Debian Repository

This is the repository that I use for publishing application packages.

### Setup Repository

```markdown
wget -O - http://adelolmo.github.io/andoni.delolmo@gmail.com.gpg.key | sudo apt-key add -
echo "deb http://adelolmo.github.io xenial main" | sudo tee /etc/apt/sources.list.d/adelolmo.list
```