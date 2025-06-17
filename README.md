# Provisionamento de Infraestrutura com Vagrant e Ansible

Este projeto demonstra a aplicação de práticas DevOps com foco em **Infraestrutura como Código (IaC)**, utilizando **Vagrant** e **Ansible** para provisionar automaticamente uma máquina virtual Ubuntu, instalar o servidor web NGINX e realizar o deploy de um site estático.

---

## 🚀 Visão Geral

Durante o bootcamp DevOps promovido pela Escola Atlântico Avanti, desenvolvi este laboratório com o objetivo de consolidar conhecimentos sobre automação de infraestrutura e provisionamento de ambientes. O ambiente provisionado simula a entrega de um servidor web configurado de forma automatizada e reproduzível.

---

## 🛠️ Tecnologias Utilizadas

- **Vagrant** – para criação e gerenciamento da máquina virtual  
- **Ansible** – para provisionamento e configuração automatizada  
- **VirtualBox** – como provedor de máquinas virtuais  
- **Ubuntu 20.04 LTS** – sistema operacional da VM  
- **NGINX** – servidor web para deploy do site estático

---

## 📦 Funcionalidades

- Criação de VM com Vagrant
- Redirecionamento de portas (8080 → 80)
- Provisionamento com Ansible local
- Instalação automatizada do NGINX
- Deploy automatizado de página web via módulo `copy`
- Suporte a handler para reinício automático do serviço NGINX

---

## ▶️ Como Executar

```bash
# Clone o repositório
git clone https://github.com/felipeomelodev/iac-with-vagrant-and-ansible.git
cd iac-with-vagrant-and-ansible

# Suba a VM provisionada
vagrant up

# (Opcional) Acesse a VM via SSH
vagrant ssh

# Acesse o site local
http://localhost:8080

# (Opcional) Reprovisione após alterações no playbook
vagrant provision

# Destrua a VM quando não for mais necessária
vagrant destroy -f
```

---

## 📄 Referências

- [Documentação do Vagrant](https://developer.hashicorp.com/vagrant/docs)
- [Documentação do Ansible](https://docs.ansible.com/)
- [Documentação do VirtualBox](https://www.virtualbox.org/wiki/Documentation)
