# RTPEngine

Role used to install RTPEngine.

## Role Variables

Variables used to control role behavior.

|            variable            |                              description                              |                       default value                                      |
| ------------------------------ | --------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| version                        | Source branch of the application source code.                         | mr9.2.1                                                                  |
| repository                     | Repository to download the source code                                | https://github.com/sipwise/rtpengine.git                                 |
| bcg729.source                  | Repository to download the source code of bcg729                      | https://codeload.github.com/BelledonneCommunications/bcg729/tar.gz/1.0.4 |
| bcg729.debian                  | Repository to download the debian settings of bcg729 package          | https://github.com/ossobv/bcg729-deb.git                                 |

## Example Playbook

Here is a small example of how to use this role:

```yml
- hosts: all
  roles:
    - role: rtpengine
      version: mr9.2.1
```

## Tests

The following stack of tools were used to test this role:

- [Virtualbox](https://www.virtualbox.org/) and [Vagrant](https://www.vagrantup.com/) for provisioning environments.

### Steps

In `tests` folder, run the commands below:

```bash
vagrant up
vagrant ssh
cd /vagrant/test
ansible-playbook test.yml
```

## Author

| [<img src="https://avatars0.githubusercontent.com/u/26543872?v=3&s=115"><br><sub>@Otoru</sub>](https://github.com/Otoru) |
| :----------------------------------------------------------------------------------------------------------------------: |
