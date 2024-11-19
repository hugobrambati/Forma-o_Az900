# Az-900
#Formação Microsoft AZ-900

_Computação em Nuvem:_ A computação em nuvem refere-se à entrega de serviços de computação (como servidores, armazenamento, bancos de dados, rede, software, etc.) pela internet ("nuvem"), permitindo que as empresas e indivíduos acessem recursos de TI sem a necessidade de manter uma infraestrutura física no local. Ela oferece flexibilidade, escalabilidade e redução de custos operacionais, permitindo que as organizações paguem apenas pelos recursos que usam, conforme a demanda.

**Modelos de Nuvem:** Existem três principais modelos de entrega de serviços em nuvem:

***IaaS (Infrastructure as a Service):*** Fornece recursos de infraestrutura, como servidores virtuais, armazenamento e redes, permitindo que os usuários gerenciem sistemas operacionais e aplicativos. Exemplo: Microsoft Azure, AWS EC2.

***PaaS (Platform as a Service):*** Oferece uma plataforma que facilita o desenvolvimento, execução e gerenciamento de aplicativos sem que o usuário precise gerenciar a infraestrutura subjacente. Exemplo: Azure App Services, Google App Engine.

***SaaS (Software as a Service):*** Fornece aplicativos prontos para uso acessados pela web, sem a necessidade de instalação ou manutenção local. Exemplo: Office 365, Google Workspace.

***CAPEX (Capital Expenditure):*** CAPEX refere-se a despesas de capital, ou seja, investimentos feitos em ativos físicos de longo prazo, como servidores, equipamentos de TI, e infraestrutura. Empresas que utilizam CAPEX fazem grandes investimentos iniciais para adquirir ou melhorar ativos tangíveis, com a expectativa de que esses ativos trarão retornos financeiros a longo prazo.

***OPEX (Operational Expenditure):*** OPEX refere-se a despesas operacionais, ou seja, custos recorrentes relacionados à operação do dia a dia do negócio, como pagamentos mensais por serviços de nuvem, manutenção e salários. A vantagem do modelo OPEX é que as empresas podem pagar por recursos conforme o uso, sem a necessidade de grandes investimentos iniciais. Ao adotar soluções em nuvem, as empresas geralmente migram de CAPEX para OPEX, aproveitando o modelo de pagamento sob demanda.

Relação entre os conceitos: A computação em nuvem permite que as empresas migrem de um modelo de CAPEX (onde elas precisam adquirir e manter hardware e infraestrutura física) para um modelo de OPEX, pagando apenas pelo uso de recursos na nuvem. Isso proporciona maior flexibilidade financeira e operativa.


#Principais Elementos de um SLA da Azure:
Garantia de Disponibilidade:

O SLA define a disponibilidade do serviço, ou seja, a porcentagem de tempo que o serviço estará operacional. Por exemplo, a Azure garante 99,99% de tempo de atividade para muitos de seus serviços, como máquinas virtuais em uma configuração de disponibilidade.
Tempo de Inatividade Permitido:

Baseado na porcentagem de disponibilidade, o SLA calcula quanto tempo de inatividade é permitido dentro de um período de 30 dias. Para um SLA de 99,99%, por exemplo, o tempo de inatividade permitido é de 4,38 minutos por mês.
Redundância e Tolerância a Falhas:

A Azure oferece redundância (backup) e tolerância a falhas em muitos de seus serviços para garantir a continuidade dos serviços. Dependendo da configuração, a disponibilidade do serviço pode ser aumentada utilizando múltiplas instâncias ou regiões geográficas.
Compensação e Créditos:

Se a Microsoft Azure não atingir os níveis de SLA acordados, o cliente pode ser elegível para créditos de serviço. Esses créditos são uma compensação financeira, que podem ser aplicados na fatura mensal do cliente.
Cobertura de SLA por Serviço:

Cada serviço da Azure tem um SLA próprio. Por exemplo, para máquinas virtuais (VMs) em uma configuração de disponibilidade, o SLA é de 99,99%, enquanto para outros serviços, como o Azure Storage, o SLA pode ser de 99,9% a 99,99%, dependendo da configuração escolhida.
Exclusões e Limitações:

O SLA geralmente inclui exclusões que detalham situações em que a Microsoft não é responsável pela falha de serviço, como falhas devido a ações do cliente, ataques cibernéticos, ou manutenção programada. Esses detalhes são importantes para entender quando o SLA não será aplicado.
Exemplos de SLA da Azure:
Máquinas Virtuais (VMs): 99,99% de tempo de atividade, se configurado com dois ou mais discos e utilizando a redundância de disponibilidade.
Armazenamento de Blobs (Azure Blob Storage): 99,9% a 99,99%, dependendo da configuração.
Azure SQL Database: 99,99% de tempo de atividade para bancos de dados na camada de Alta Disponibilidade.
Conclusão:
O Acordo de Nível de Serviço (SLA) da Azure é uma parte crucial para garantir que os clientes saibam o que esperar em termos de disponibilidade e confiabilidade dos serviços. É importante que as empresas compreendam os SLA de cada serviço que utilizam, pois isso impacta diretamente a performance e os custos associados à utilização dos recursos da nuvem.

Configurando um banco de dados na Azure

Passos para Criar e Configurar uma Instância de Banco de Dados na Azure:
1. Criar uma Conta e Entrar no Portal da Azure
Acesse o Portal da Azure.
Se você não tiver uma conta, crie uma gratuitamente.
Após o login, você será direcionado ao painel principal do portal.
2. Criar um Novo Banco de Dados
No painel principal, clique em "Criar um Recurso" no canto superior esquerdo.
Em seguida, selecione "Banco de Dados" ou "Azure SQL Database", dependendo do banco que você deseja criar.
3. Escolher o Tipo de Banco de Dados
Azure SQL Database: Ideal para bancos de dados SQL gerenciados.
Cosmos DB: Para bancos NoSQL e dados globais.
MySQL ou PostgreSQL: Se preferir usar outros tipos de banco de dados SQL.
4. Configuração do Banco de Dados
Após selecionar o tipo de banco de dados (por exemplo, Azure SQL Database), você precisará configurar os parâmetros da instância:

Nome do Banco de Dados: Escolha um nome único para o banco de dados.
Assinatura: Selecione a assinatura da Azure onde o banco será criado.
Grupo de Recursos: Selecione um grupo de recursos existente ou crie um novo para organizar os recursos relacionados.
Localização: Escolha a região onde o banco de dados será hospedado (ex: "East US", "West Europe").
Plano de Preço: Escolha o plano de desempenho do banco (ex: "Basic", "Standard", "Premium"). Isso determina a quantidade de recursos de CPU, memória e armazenamento disponíveis.

5. Configuração de Rede
Configuração de Firewall: Para garantir a segurança, você precisará configurar as regras de firewall para permitir conexões à instância do banco. Você pode restringir o acesso aos IPs da sua rede ou permitir acessos públicos dependendo da necessidade.
VNET (Virtual Network): Se você precisar de um banco de dados que faça parte de uma rede virtual privada, configure a conexão com a VNET.

6. Configuração de Backup e Recuperação
Backup Automático: A Azure oferece backups automáticos de banco de dados, que podem ser configurados com a política de retenção de dados (ex: 7, 14, 30 dias).
Recuperação Geo-Redundante: Você pode configurar replicação geográfica para garantir que o banco de dados esteja disponível mesmo se uma região da Azure falhar.

7. Configuração de Escalabilidade
Escalabilidade Vertical: A Azure permite alterar a performance do banco de dados conforme a demanda, ajustando o plano de preço ou as configurações de vCores e armazenamento.
Escalabilidade Horizontal: Se precisar de mais instâncias do banco, você pode usar a funcionalidade de Sharding ou configurar réplicas para distribuir a carga.

8. Criar e Configurar o Usuário Administrador
Defina o nome de usuário administrador e a senha do banco de dados. Esse usuário será responsável pela administração da instância, criação de tabelas, e gestão de permissões.

9. Revisão e Criação
Após revisar todas as configurações, clique em Criar para provisionar a instância de banco de dados.

10. Conectar-se ao Banco de Dados
Após a criação, a Azure fornecerá uma string de conexão que você pode usar para conectar-se ao banco de dados. A string inclui informações como o nome do servidor, nome do banco de dados, e credenciais de acesso.
Use ferramentas como SQL Server Management Studio (SSMS), Azure Data Studio, ou até mesmo uma aplicação de software para conectar ao banco de dados e começar a interagir com ele.

11. Gerenciar e Monitorar
Após a criação, você pode monitorar o desempenho do banco de dados, realizar ajustes de configuração e ver métricas de uso (CPU, I/O, memória) diretamente pelo Azure Portal.
Além disso, é possível configurar Alertas para notificá-lo sobre questões como utilização excessiva de recursos ou falhas.

Conclusão:
Criar e configurar uma instância de banco de dados na Azure envolve etapas como a criação do banco de dados no portal da Azure, configuração de parâmetros de rede e segurança, escolha de planos de desempenho, e conexão ao banco. A Azure também oferece opções de escalabilidade, backups automáticos e monitoramento para garantir a disponibilidade e performance do banco de dados.

