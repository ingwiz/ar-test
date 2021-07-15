## ar-test
# Simple test docker and ansible

Server OS: Centos 7.9

Preparing and running.

1. Make sure that you have access to the server using a public key with root user rights
2. Install the code to workstation:
````
git clone https://github.com/ingwiz/ar-test.git
````
3. Change working dir
````
cd ar-test/ansible
````
4. Specify the Server host IP in the file `inventory/prod` in the variable `ansible_ssh_host`
5. Run playbook
````
ansible-playbook -i inventory/prod build-and-run.yml
````
6. Testing
````
curl http://<server-ip>:8081
````
