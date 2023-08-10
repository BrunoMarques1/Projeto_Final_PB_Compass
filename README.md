# Arquitetura Fast Engineering S/A
### Escopo: 
Realizar a construção e implementação do ambiente de servidores da empresa "Fast Engineering S/A" para a AWS, utilizando as melhores práticas DevOps e garantindo alta disponibilidade, escalabilidade e segurança.

### Arquitetura:
- Ambiente Kubernetes (EKS): Utilizar o serviço Amazon Elastic Kubernetes Service (Amazon EKS) para orquestrar e gerenciar os contêineres da aplicação em um ambiente altamente disponível e escalável.
- Banco de dados PaaS: Utilizar o serviço Amazon Relational Database Service (Amazon RDS) para hospedar o banco de dados MySQL. O RDS oferece gerenciamento automatizado, escalabilidade e backups automáticos.
- MultiAZ: Configurar o RDS com alta disponibilidade MultiAZ, garantindo que haja réplicas do banco de dados em diferentes zonas de disponibilidade para tolerância a falhas. 
- Persistência dos Dados: Utilizar o EBS (Elastic Block Store) para fornecer armazenamento persistente aos contêineres e garantir que os dados estejam seguros mesmo após a reinicialização das instâncias.
- Balanceamento de carga com healthcheck: Implementar o Amazon Elastic Load Balancing (ELB) para distribuir o tráfego de entrada entre as instâncias do contêiner, realizando healthchecks para verificar a disponibilidade dos serviços.
- Segurança: Configurar grupos de segurança da AWS para restringir o acesso apenas aos serviços e portas necessários, garantindo a segurança do ambiente. Além dos grupos de segurança, o IAM também será configurado para gerenciar as permissões e acesso aos recursos da AWS. Serão criados grupos de usuários e políticas de acesso que permitem apenas o mínimo necessário para cada serviço e função na empresa.
- Resolução de Nomes e DNS (Amazon Route 53): Utilizar o Amazon Route 53 para gerenciar o DNS da empresa. Isso inclui a resolução de nomes de domínio, a criação de registros DNS, a configuração de zonas hospedadas e a rota de tráfego de entrada para os serviços hospedados na AWS, garantindo alta disponibilidade e latência mínima.

<div align="center">
  
![image](https://github.com/BrunoMarques1/Projeto_Final_PB_Compass/assets/127341401/4e1a5c27-b343-4477-9435-bbef8ef08d17)


</div>

### Valores:
A estimativa mensal de gastos dessa arquitetura ficou em torno de 755.00 USD, enquanto a anual ficou em 9,070.00 USD (Lembrando que os valores podem variar dependendo da carga e demanda).

### Prazo de entrega:
Para a realização e implementação integral dos serviços oferecidos pela empresa Fast Engineering S/A, estima-se que seja necessário um período aproximado de duas semanas.

### Cronograma de macro-integras:
- Prova de conceito (POC): A POC servirá para validar a arquitetura criada, expondo possíveis falhas e indicando possíveis mudanças antes de criarmos o MVP. Para a prova de conceito será necessário 3 dias e meio.
- Mínimo produto viável (MVP): Na MVP, teremos apenas os recursos mínimos, com suas funcionalidades básicas, sendo assim uma versão enxuta do Produto final. Para a criação do Mínimo produto viável será necessário 3 dias e meio.
- Produto final: O produto final será a implementação da arquitetura apresentada. Para construir a arquitetura apresentada, será necessário aproximadamente uma semana.


