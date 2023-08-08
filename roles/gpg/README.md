gpg:  ## setup gpg config
gpg: .gnupg/gpg-agent.conf
gpg: /etc/ssh/sshd_config
	chmod 0700 .gnupg
#gpg: .gnupg/pubring.kbx
#gpg: .gitconfig.user

.gnupg/gpg-agent.conf::
	echo "enable-ssh-support" > $@
