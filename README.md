<h1 align="center">Projeto - Monitoramento</h1>

<h2>Objetivo:</h2>

Realização de monitamento de 2 maquinas, sendo a máquina local e uma máquina virtual (VM).

Para isso, foi necessário:

    • Inicialização de uma máquina Linux utilizando o vagrant (ubuntu – última versão)
    • Criar um usuário e também criar uma chave ssh para o usuario (chave.pem ou chave.ppk).
    • Acessar a máquina remotamente através do “putty” utilizando a chave ssh gerada.
    • Atualizar todos os pacotes do SO para correção de problemas de Segurança e bugs.
    • Instalar o apache e subir uma página de “Hello World”
    • Habilitar e desabilitar o Firewall (Liberar as portas exclusivas da aplicação)
    • Habilitar “logrotate” (alterar a configuração para rotacionar por 7 dias e compactar)
    • Garantir que o apache inicialize automaticamente após o reboot da máquina virtual 
    • Adicionar um novo disco de 2GB e realizar a montagem dele na máquina virtual no diretorio /usr/local/meu_nome


Após a conclusão da configuração da VM, realizei a monitoração de nosso ambiente de infraestrutura, utilizando as ferramentas abaixo:

    · Instalar o zabbix na máquina Linux.
    · Instalar um Agent na máquina virtual (linux)
    · Instalar um Agent na máquina pessoal.
    · Criar uma monitoração de webscenário da url “Hello World” - Monitoração Sintética
    · Habilitar a coleta de metricas de sistemas Operacionais. (CPU, memória , swap, disco e inode)
    · Instalar o Grafana na máquina Linux e ativar a integração com o zabbix.
  
Ao final, criei um dashboard contendo:

    o Status up/down dos servidores.
    o Consumo de recurso de CPU
    o Consumo de memória
    o Consumo de disco.
    o Consumo de Swap
    o Consumo de inode

<h2>Ferramentas Utilizadas:</h2>

    ● Vagrant;
    ● Zabbix;
    ● Grafana;
    ● Kanban;
    ● Scrum;

<h2>Arquitetura:</h2>

![image](https://user-images.githubusercontent.com/116106336/196504638-1908b1f4-da33-449f-81eb-b0783aec102e.png)


<h2>Zabbix:</h2>

![image](https://user-images.githubusercontent.com/116106336/196509447-07b3ff72-c9b5-4d05-9b62-7b15261dc848.png)

![image](https://user-images.githubusercontent.com/116106336/196509562-8ac61c9f-4c24-40e1-b0b5-dda2b406693a.png)


<h2>Grafana:</h2>

![image](https://user-images.githubusercontent.com/116106336/196509222-b67d1019-6416-44c8-a8ff-e2624ad3080f.png)

![image](https://user-images.githubusercontent.com/116106336/196509366-fd461a24-2c4c-4334-86b0-5f830efef05e.png)

<h2>Kanban - Métricas Corello:</h2>

![image](https://user-images.githubusercontent.com/116106336/196509816-dca52d72-5ace-42ad-81fd-aa153e06383d.png)

![image](https://user-images.githubusercontent.com/116106336/196509866-2fff97b3-24ea-4570-be1c-66db2b2db55a.png)
