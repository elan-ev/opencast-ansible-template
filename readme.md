deploy opencast

    ansible-playbook --ask-vault-pass -i inventory/server.hosts install-opencast-allinone.yml --limit test

generate password

    pwgen -n1 42

create and edit ansible vaults

    ansible-vault create group_vars/test.yml
	 ansible-vault edit group_vars/test.yml
