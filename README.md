# nginx-tls-webserver-playbook
Vagrant and Ansible project to create a VM and provision it with a basic NGINX webserver, on a https conection.

**Prerequisites:**
- python3
- vagrant
- ansible
- oracle virtualbox, for virtualization vagrant support (or any other virtualization software: VMWare, KVM, etc.)

**Run:**
- `vagrant up` -> create VM on VirtualBox with the specs inside Vagrantfile
- `ansible nginx-tls-w-role.yml` -> provision the VM with nginx webserver, a basic website and a TLS self signed certificate.
- check inside your browser: http://localhost:8443/index.html
