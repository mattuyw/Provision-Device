ansible-playbook -i /opt/new-device-setup/inventory/dba.ini -K site.yml

; my-instance ansible_host=i-0aa2a0488cc6096c9
;
; [all:vars]
; ansible_ssh_common_args=-o StrictHostKeyChecking=no -o ProxyCommand="sh -c \"aws ssm start-session --target %h --document-name AWS-StartSSHSession --parameters 'portNumber=%p'\""
; ansible_user='mattuyw'

Need to set up a temporary SSH key ahead of time.
Clone dotfiles
xcode-select --install
cd /tmp
python3 -m venv .venv
. .venv/bin/activate
pip install ansible
