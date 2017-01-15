# ansible-vagrant-tutorial

#### SSH login without password

Let's assume we want to create a passwordless connection between Bob and Alice (Bob connects Alice):

- From Bob's machine,
    `ssh-keygen -t rsa`
    
- Copy `~/.ssh/id_rsa.pub` file from *Bob's* machine and paste it on `.ssh/authorized_keys` in *Alice's machine*
