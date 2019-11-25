 role fuse/sshfs
=================
Ansible role to manage fuse/sshfs

This role install sshfs and will mount all configured mounts to the configured folders.

### required config:
```
sshfs:
  - server: example.com
    user: pi
    remote: /home/pi/backup
    local: /mnt/example.com
  - server: www.example.com
    user: debian
    remote: /home/debian/backup
    local: /mnt/www.example.com
```

For more config options and features have a look into the defaults folder!

### galaxy
```
# install role via ansible-galaxy:
ansible-galaxy install do1jlr.role_sshfs
```
