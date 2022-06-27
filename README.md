# Arch Linux System Packages Repo
> Note: This page is auto generated!

## Init Install scripts
```bash
curl -sL https://arch.packages.project0.de/key.asc | pacman-key -a
pacman-key --lsign-key 7DE840C6D3BDFEDC
curl https://arch.packages.project0.de/bin/install.sh -o /tmp/project0-bootstrap-install.sh
curl https://arch.packages.project0.de/bin/disk.sh -o /tmp/project0-bootstrap-disk.sh
chmod a+x /tmp/project0-bootstrap-install.sh /tmp/project0-bootstrap-disk.sh
# Setup disk: /tmp/project0-bootstrap-disk.sh /dev/disk <true:encrypt>'
# Install arch: /tmp/project0-bootstrap-install.sh https://arch.packages.project0.de'
```

## Pacman config
```ini
[project0-system]
Server = https://arch.packages.project0.de/$repo

[project0-aur]
Server = https://arch.packages.project0.de/$repo

[project0-packages]
Server = https://arch.packages.project0.de/$repo
```

## Key
Fingerprint `7DE840C6D3BDFEDC`

[Public Key](https://arch.packages.project0.de/key.asc)
```bash
curl -sL https://arch.packages.project0.de/key.asc | gpg
curl -sL https://arch.packages.project0.de/key.asc | sudo pacman-key -a
sudo pacman-key --lsign-key 7DE840C6D3BDFEDC
```
