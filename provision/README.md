# My Laptop Provision Playbooks

> Set of [Ansible](https://www.ansible.com/) playbooks to provision a Fedora machine with all my applications and settings.

## Pre-requisites

* A machine running Fedora OS. This playbook was tested with Fedora 32.
* Git (`dnf install -y git`)
* GitHub personal access token. You can get one [here](https://github.com/settings/tokens).

## Initial Setup

To provision a new machine open a terminal window and run the following commands:

```sh
export GITHUB_TOKEN=<my_github_token>
git clone https://github.com/brpaz/my-linux-setup
sudo chmod +x setup.sh
./setup.sh
```

**Note** When installing dotfiles you will be prompted for the "pgp" key to decrypt the secure files. Make sure to have it at hand.

### Manual Steps

Unfortunately not everything can be automated and some manual steps will be required after running this scripts.

* Execute Jetbrains toolbox and install the IDEs
* Open Web browser and enter the "Sync Password" to sync all the extensions, bookmarks etc.
* Install [DevDocs Desktop](https://github.com/hardpixel/devdocs-desktop) and enable docsets
* Install [Ulauncher Extensions](https://ext.ulauncher.io/)
* Login into applications (Spotify, etc).
* Install Graphics Drivers

---

## Keep the system updated

Most of the tasks are idenpotent and you can use this playbook to keep your system updated. This is useful, for example, to automatically update all the programs installed from GitHub, as the playbooks will try to fetch and install always the latest release.

You can execute a specific tag, by running:

```
 TAG=node make run-tag
```

---

## TODO

* Fix ansible lint warnings and improve idenpontency of some tasks

---

## Reference

* http://radeksprta.eu/automatically-setup-computer-ansible-playbook/
* http://blog.josephkahn.io/articles/ansible/
* https://github.com/Benoth/ansible-ubuntu

## Author

👤 **Bruno Paz**

* Website: [brunopaz.dev](https://brunopaz.dev)
* Github: [@brpaz](https://github.com/brpaz)

## 📝 License

Copyright © 2019 [Bruno Paz](https://github.com/brpaz).

This project is [MIT](https://opensource.org/licenses/MIT) licensed.

