### commands to run playbook ###

# creates ec2 key pair, security group, ec2 instance, postgres rds instance
ansible-playbook ec2.yml -e ansible_python_interpreter=/usr/bin/python3

# configure server with python3, docker, docker-composem, copy docker-compose.yml and start containers
ansible-playbook app.yml -i hosts

## extra credit ##
ansible-playbook alb.yml -e ansible_python_interpreter=/usr/bin/python3
