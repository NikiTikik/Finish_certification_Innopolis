# Finish Certification
It's a playbook for certification in DevOps course of Innopolis university

Firstly, this playbook will install Docker and nginx,
then it will configure nginx and run docker container with web application (simple file loader)
(you can access web application via IP of host)

Moreover, playbook install elasticsearch, kibana and filebeat
(you can access kibana on port 5601 to monitore nginx)

For correct work you need to change two varibles:
in file "ubuntu-servers" enter address of your web-server
in file roles/nginx/vars/main.yml change public ip-address of your web-server

You only need to run the command:
ansible-playbook -i ubuntu-servers play.yml
