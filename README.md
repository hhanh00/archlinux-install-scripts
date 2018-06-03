Install scripts for Archlinux

# Requirements

- public key in .ssh/id_rsa.pub
`ssh-keygen -y -f id_rsa > id_rsa.pub`
- Modify the scripts to match your configuration
  - in `run.sh` PORT, HOST
  - in `install.sh`: mirror location
  - in `chroot.sh`: hostname, user, locale, timezone, 

# Tested in Virtualbox

- Insert installation iso and boot to root prompt
- Run in the installed machine prompt
```
paswswd
systemctl start sshd
```
- Run in the source machine
`./run.sh`
