# commands
- aws ec2 describe-instances --query 'Reservations[*].Instances[*].PublicIpAddress' --output text >> inventory
- ansible-playbook main-remote.yml -i inventory --private-key ancible.pem