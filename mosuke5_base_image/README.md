# mosuke5's base image with Packer
This is the example for creating image for my own with Packer.

```
$ export ALICLOUD_ACCESS_KEY=xxxxxxxxxxx
$ export ALICLOUD_SECRET_KEY=xxxxxxxxxxx
$ export GITHUB_NAME=mosuke5

$ packer build packer.json
```

The image which this code will create contain following.

1. Ansible install
1. Execute ansible playbook
    1. Create general user
    1. Add general user to sudoers
    1. Set my public keys from github
    1. Change ssh settings
