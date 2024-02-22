# Install Asterisk

## Saltstack
This method describes using Saltstack formula [asterisk-formula][formula] to install Asterisk.

We will use [salt-call][salt-call] command, a standalone saltstack minion process to process `asterisk-formula` and install asterisk.

```sh
pip3 install salt
git clone https://github.com/litnialex/asterisk-formula.git
salt-call -l info --local --file-root=asterisk-formula/ state.apply asterisk
```


## Ansible
This method describes using Ansible playbook to install Asterisk.


[formula]: https://github.com/litnialex/asterisk-formula
[salt-call]: https://docs.saltproject.io/en/latest/ref/cli/salt-call.html
