# Redução dos Custos em Farmácias com AWS #
Repositório para o curso Redução dos Custos em Farmácias com AWS, que visa criar um relatório apresentando serviços AWS para redução de custos.

# RELATORIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS #
Data: 01/09/2025

Empresa: Abstergo Industries

Responsável: Ícaro Sanches

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo, realizado por Ícaro Sanches. O objetivo do projeto foi elencar 5 serviços AWS, com a finalidade *realizar diminuição de custos imediatos.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:

Etapa 1:
- Instâncias EC2
- Provisionamento de máquinas em nuvem.
- O uso de instâncias EC2 permite migrar máquinas de servidores físicos para máquinas em nuvem. A proposta das instâncias EC2 permitem redução de custos com implementação e manutenção de infraestrutura física. Além disso, as máquinas podem ser criadas com configurações e volumes de tipos diferentes, permitindo fácil adequação a diferentes contextos do projeto, como armazenamento de dados ou processamento de transações financeiras. Também permite redundância e escalonamento automático, diminuindo a possibilidade de instabilidade e perdas.

Etapa 2:
- Elastic Load Balance (ELB)
- Realiza o balanceamento de tráfego. 
- Considerando a utilização de múltiplas máquinas EC2, o ELB permite roteamento avançado de tráfego, distribuindo a carga entre as máquinas de maneira mais otimizada. Também permite testar a conexão com uma máquina na rede interna e em caso de falha, encaminhar para outra. Desta forma, as chances de uma máquina ficar sobrecarregada, enquanto outra está sem carga é reduzida. Também reduz a chance de indisponibilidade do sistema ao testar as conexões. Com um Load Balancer configurado, o desempenho dos servidores pode ser otimizados, o que pode levar a redução de custos.

Etapa 3:
- VPC Security Group
- Segurança de rede
- Security Groups atuam com firewalls virtuais que controlam o tráfego entre recursos AWS. Controla tanto o tráfego de entrada quanto de saída das instâncias, dessa maneira verifica quem pode ou não acessar um recurso e o que está saindo. No sistema, garantiria segurança e separaria acessos, fazendo com que um servidor de controle de estoque não tenha acesso à um servidor de frente de caixa e vice e versa. 

Etapa 4:
- Amazon RDS e DynamoDB
- Bancos de dados
- Um sistema de comércio possui necessidade de db's SQL convencionais, uma vez que transações financeiras precisam ser registradas de forma estruturada. Desta forma, o Amazon RDS atende a necessidade. Já o DynamoDB, um banco NoSQL, permite armazenamento com flexibilidade de esquema e baixa latência. Desta forma, em uma rede de comércio que possui necessidade de consultas de estoque ou pode precisar de mudanças do esquema entre diferentes filiais, o uso de bancos NoSQL traz benefícios.  

Etapa 5:
- Bucket S3
- Armazenamento de Logs
- Considerando a necessidade de registros de log das instâncias e recursos, o S3 se apresenta como uma boa alternativa pois permite integração nativa com outros ambientes AWS, altíssimas durabilidade e escalabilidade dos dados e baixo custo. Desta forma, com este recurso, o tempo e a facilidade para identificação de possíveis problemas podem ser otimizados.  

## Conclusão ##
A implementação de ferramentas na empresa *Abstergo tem como esperado otimização de recursos, redução de custos, escalabilidade, armazenamento robusto, controle e segurança*, o que aumentará a eficiência e a produtividade da empresa. Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa.

## Anexos ##

### Documentação oficial Amazon ###
* [Amazon EC2](https://aws.amazon.com/pt/ec2/?nc2=h_prod_cp_ec2)
* [Elastic Load Balancing](https://aws.amazon.com/pt/elasticloadbalancing/?nc2=h_ql_prod_nt_elb)
* [Amazon VPC](https://aws.amazon.com/pt/vpc/?nc2=h_ql_prod_fs_vpc)
* [Amazon RDS](https://aws.amazon.com/pt/rds/?nc2=h_ql_prod_fs_rds) & [DynamoDB](https://aws.amazon.com/pt/dynamodb/?nc2=h_ql_prod_fs_ddb)
* [Amazon S3](https://aws.amazon.com/pt/s3/?nc2=h_ql_prod_fs_s3)

---

Assinatura do Responsável pelo Projeto:

Ícaro Sanches