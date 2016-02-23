# A Lot to Love

## Getting started

This project is using [Codeup's Vagrant VM]
(https://github.com/gocodeup/Codeup-Vagrant-Setup). The simplest way to set it
up is by downloading the
[clickable installer](https://github.com/gocodeup/LAMP-Setup-Script/archive/master.zip)
if your using OS X.

Once you have everything installed clone this repository inside
`~/Codeup-Vagrant-Setup/sites`.

```bash
$ git clone git@github.com:codeforsanantonio/a_lot_to_love.git alottolove.dev
```

Run the following Ansible playbook (enter `alottolove.dev` when prompted to
enter a Domain name).

```bash
$ ansible-playbook ansible/playbooks/vagrant/site/php.yml
```

Open your `/etc/hosts` file in your preferred editor (you might need to use
`sudo`). Add the following line at the end of the file.

```
 192.168.77.77 alottolove.dev
```

Browse to [alottolove.dev](http://alottolove.dev) to verify everything works.

## How To Contribute

Fork this repository and send your Pull Request to the `master` branch.

## License

[MIT](LICENSE)
