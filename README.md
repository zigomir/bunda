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

## Infrastructure notes

### GitHub repos

- [client aka tripster](https://github.com/zigomir/tripster)
- [server aka flyout](https://github.com/zigomir/flyout)
- [authorization service aka proxio](https://github.com/zigomir/proxio) - was previously proxying requests from client to server

## TODO - neverending updates

- ruby 2.1.2 (when on ppa:brightbox/ruby-ng)
- [ubuntu 14.04 + passenger 4.0.42](http://blog.phusion.nl/2014/05/07/phusion-passenger-4-0-42-released-ubuntu-14-04-packages-available/)
