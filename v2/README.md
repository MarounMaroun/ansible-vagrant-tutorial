# ansible-vagrant-tutorial

#### Adding key in inventory file

By default, SSH looks for the key in `~/.ssh/id_rsa`, but let's assume it doesn't, and let's tell andible where our private key is located. 

There are many options to do that, we will copy the content of `~/.ssh/id_rsa` to `/etc/ansible/keys/web.pem`, and add the following to the `hosts` file:

```
[webservers:vars]
ansible_ssh_private_key_file=/etc/ansible/keys/web.pem
```

That's all!

