# ar-test
<h1> Simple test docker and ansible </h1>

Preparing.
1. Make sure that you have access to the server using a public key with root user rights
2. Install the code to workstation:
````
git clone https://github.com/ingwiz/ar-test.git
````
3. Set working dir
````
cd ar-test/ansible
````
4. Specify the Server host IP
````
vi inventory/prod
````
5. Run playbook
````
ansible-playbook -i inventory/prod build-and-run.yml
````
6. Testing
````
curl http://<server-ip>:8081
````
