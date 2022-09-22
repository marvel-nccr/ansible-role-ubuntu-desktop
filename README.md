[![CI](https://github.com/marvel-nccr/ansible-role-ubuntu_desktop/workflows/CI/badge.svg)](https://github.com/marvel-nccr/ansible-role-ubuntu_desktop/actions)
[![Ansible Role](https://img.shields.io/ansible/role/35372.svg)](https://galaxy.ansible.com/marvel-nccr/ubuntu_desktop)
[![Release](https://img.shields.io/github/tag/marvel-nccr/ansible-role-ubuntu_desktop.svg)](https://github.com/marvel-nccr/ansible-role-ubuntu_desktop/releases)

# Ansible Role: marvel-nccr.ubuntu_desktop

Description...

## Installation

`ansible-galaxy install marvel-nccr.ubuntu_desktop`

## Role Variables

See `defaults/main.yml`

## Example Playbook

```yaml
- hosts: servers
  roles:
  - role: marvel-nccr.ubuntu_desktop
```

## Development and testing

This role uses [Molecule](https://molecule.readthedocs.io/en/latest/#) and [Docker](https://www.docker.com/) for tests.

After installing [Docker](https://www.docker.com/):

Clone the repository into a package named `marvel-nccr.ubuntu_desktop` (the folder must be named the same as the Ansible Galaxy name)

```bash
git clone https://github.com/marvel-nccr/ansible-role-ubuntu_desktop marvel-nccr.ubuntu_desktop
cd marvel-nccr.ubuntu_desktop
```

Then run:

```bash
pip install -r requirements.txt  # Installs molecule
molecule test  # runs tests
```

or use tox (see `tox.ini`):

```bash
pip install tox
tox
```

## Code style

Code style is formatted and linted with [pre-commit](https://pre-commit.com/).

```bash
pip install pre-commit
pre-commit run -all
```

## Deployment

Deployment to Ansible Galaxy is automated *via* GitHub Actions.
Simply tag a release `vX.Y.Z` to initiate the CI and release workflow.
Note, the release will only complete if the CI tests pass.

## License

MIT

## Contact

Please direct inquiries regarding Quantum Mobile and associated ansible roles to the [AiiDA mailinglist](http://www.aiida.net/mailing-list/).
