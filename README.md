# Projeto de Estudos do Ansible #ChamaAsMina

## Pré-Requisitos
* Python 2.7
* Ansible 2.6

## Pacote de Provisioning das Máquinas do Cluster
Para instalar o Helm nos hosts desejados execute o comando abaixo na pasta do pacote chamado `provisioning`:
```
ansible-playbook -i hosts main.yml
```

## Pacote de Instalação e Configuração do Cluster
Após a execução do `provisioning`, devemos pegar os ips das máquinas criadas na AWS e preencher no arquivo de `hosts` para instalação do k8s existente na pasta `install_k8s`.
Para instalar o Helm nos hosts desejados execute o comando abaixo na pasta do pacote chamado `install_k8s`:
```
ansible-playbook -i hosts main.yml
```

## Pacote de Instalação do Helm
Foi criado um pacote Ansible para instalação do Helm. 
Para iniciar a instalação, adicione o endereço do host desejado no arquivo para instalação do Helm.
Para instalar o Helm nos hosts desejados execute o comando abaixo na pasta do pacote chamado `install-helm`:
```
ansible-playbook -i hosts main.yml
```