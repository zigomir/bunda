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