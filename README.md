# README

Install ansible-galaxy roles:
`ansible-galaxy install -r requirements.yml`

Setup a vault password text file with the secret password
`code ~/.vault_pass.txt`

Setup vagrant for testing:
`vagrant up`

Run the playbook against vagrant:
`ansible-playbook -i vagrant_hosts.yml site.yml --vault-password-file ~/.vault_pass.txt`

Access Monit HTTP:
`ssh -L2812:localhost:2812 deploy@192.168.111.222`
