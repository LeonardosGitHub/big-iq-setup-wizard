# big-iq-setup-wizard

Ansible playbook to provision BIG-IQ based on [Ansible Galaxy f5devcentral/bigiq_onboard](https://galaxy.ansible.com/f5devcentral/bigiq_onboard)

## Directory Structure

```bash
.
├── roles
│   └── f5devcentral.bigiq_onboard
├── bigiqplaybook.yaml
├── hosts
└── vars
    └── main.yaml
```

## Sources

1. `roles/f5devcentral.bigiq_onboard` 

  Ansible Galaxy module copied from [https://galaxy.ansible.com/f5devcentral/bigiq_onboard](https://galaxy.ansible.com/f5devcentral/bigiq_onboard)

2. `bigiqplaybook.yaml`

  Playbook file created from `roles/f5devcentral.bigiq_onboard/README.md` - see section "Example Playbook"

3. `hosts`

  Sample inventory file.

  - Replace `bigiq.example.com` with the host name of the BIG-IQ host
  - Replace `1.2.3.4` with the IP of the BIG-IQ host

4. `vars/main.yaml`

  Ansible variables file copied from `roles/f5devcentral.bigiq_onboard/default/main.yaml`

  - Replace all necessary values. *** Do not commit changes ***

## Usage

```bash
ansible-playbook bigiqplaybook.yaml -i hosts
```