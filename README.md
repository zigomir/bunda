# Bunda

Build me servers; Run them on [clouds](https://www.youtube.com/watch?v=3acIH2PhMe0).

## Ansible

ALl knowledge taken from [mazer-rackham](https://github.com/jlund/mazer-rackham) and [ansible](https://github.com/eduardodeoh/ansible).

## DigitalOcean

```sh
vagrant plugin install vagrant-digitalocean
vagrant up --provider=digital_ocean


ansible production -i hosts -m ping -u root
ansible-playbook -i hosts setup_digitalocean.yml
```

## Wrong Ruby version?

Be sure to re-install `bundler` and try to run `gem` cause executables might be referenced to `ruby1.9`.

```sh
update-alternatives --set ruby
```

## TODO

Finish SSL config when we enable IP <=> jetlaggin.com on domain registrar.

## SSL all the way

[Very good source on how to get free certificates](https://konklone.com/post/switch-to-https-now-for-free)
