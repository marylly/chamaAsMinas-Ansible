# Projeto de Estudos do Ansible #ChamaAsMina

## Pré-Requisitos
* Python 2.7
* Ansible 2.6

## Pacote de Instalação do Helm

Foi criado um pacote Ansible para instalação do Helm. 
Para iniciar a instalação, adicione o endereço do host desejado no arquivo para instalação do Helm.
Para instalar o Helm nos hosts desejados execute o comando abaixo na pasta do pacote chamado `install-helm`:
```
ansible-playbook -i hosts main.yml
```