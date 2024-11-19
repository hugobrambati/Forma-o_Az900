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
