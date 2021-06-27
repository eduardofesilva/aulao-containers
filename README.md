# Tech Talenbt - Aulão Containers
Repositório criado para ilustrar alguns conceitos de containers, kubernetes e gerenciamento de configuração.

Em nenhum momento o codigo nesse repositório pode ser considerado produtivo e aplicado em ambientes de produção
# Requisitos

## Mandatórios
- EC2 - Ubuntu 18.04
- Chave SSH e Security Group aberto na porta 22, 80, 8080, 30000-32767 (Kubernetes)

## Desejável
- Terraform
- Ansible


# Ansible

# Configurações

- Para executar esse playbook você necessita fornecer o IP ou Hostname atribuido a máquina final e a localização da sua chave SSH
- Nesse aulão estou assumindo que a chave esta localizada em $HOME/.ssh/sre.pem (conforme)
- O arquivo ansible.cfg é o responsável por dizer qual é o arquivo de hosts a ser utilizado e por desabilitar o host key checking
## Executando o playbook
- Acesse o terminal de sua maquina
- Entre na pasta deste repositório
- Acesse a pasta ansible
- Execute o comando abaixo
```bash
ansible-playbook main.yml
```

# Kubernetes

## Configurando o Ingress

[Link](https://kubernetes.io/docs/tasks/access-application-cluster/ingress-minikube/)