## Ubuntu / Debian Repository

This is the repository that I use for publishing application packages.

List of current [packages](PACKAGES.md) in the repositories.

### Setup Repository

```markdown
sudo apt-get install apt-transport-https
```
For ubuntu trusty:
```
wget -O - http://adelolmo.github.io/andoni.delolmo@gmail.com.gpg.key | sudo apt-key add -
echo "deb http://adelolmo.github.io/trusty trusty main" | sudo tee /etc/apt/sources.list.d/adelolmo.list
```
For ubuntu xenial:
```
wget -O - http://adelolmo.github.io/andoni.delolmo@gmail.com.gpg.key | sudo apt-key add -
echo "deb http://adelolmo.github.io/xenial xenial main" | sudo tee /etc/apt/sources.list.d/adelolmo.list
```
For debian jessie:
```
wget -O - http://adelolmo.github.io/andoni.delolmo@gmail.com.gpg.key | sudo apt-key add -
echo "deb http://adelolmo.github.io/jessie jessie main" | sudo tee /etc/apt/sources.list.d/adelolmo.list
```
For debian stretch:
```
wget -O - http://adelolmo.github.io/andoni.delolmo@gmail.com.gpg.key | sudo apt-key add -
echo "deb http://adelolmo.github.io/stretch stretch main" | sudo tee /etc/apt/sources.list.d/adelolmo.list
```