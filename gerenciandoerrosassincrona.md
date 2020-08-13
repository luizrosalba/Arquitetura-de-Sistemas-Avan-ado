# Aprenda o que é e como funciona arquitetura em mensageria
- RestApi 
- Message Brokers 
- SErviçoes que se comunicam com o mundo externo (proxy HTTP ) 
- Serviços que nao se comunicam com o mundo externo mas recebem mensagem do MB 
Pros : 
- Desacoplamento 
- FAcil plug and play 
- comunicação assíncrona 
- Simples escalabilidade 
- broadcasting 
-Permite Event Source 
Contra 
- Single point of failure (MB quebra a arquitetura) 
- Dificil Monitoramento (toda comunicação é assíncrona) 

## Gerenciamento de Erros : 
- Dead letter queue - filas de re-tentativas (CAdastro de cobrança sem cartão de crédito cadastrado) 
- monitoramento entre serviços 
- rastreamento de fluxo 
- Armazenar os logs indexados e pegar um metadado (ex: track ID) 


## Arquitetura de dados não estruturados e business intelligence

Business Intelligence 
- Ferramentas, infraestrutura, profissionais( corpo técnico) , dados 
Bi data 
- Dados gerenciais 
- Dados da operacao 
- Pesquisa de campo 
- Indicadores de mercado 
Bi solution 
- infrastrutura 
- gerenciamento de dados 
- analytics 
- compartilhamento 
- ferramentas gerais 
Ferramentas de bi 
- Power bi 
- sas 
- sap business 
- oracle 
- microstrategy 
- tableau 
## Aprenda sobre os conceitos de Data Warehouse
- OLTP x OLAP 
Online transaction processing  (oltp)
-Operacional 
- dados voláteis passíveis de modificação e exclusão 

Online analytical processing  ( publico reduzido ) (olap) 
-estratégico 
- dados históricos nao voláteis , não sofrem alterações salvo necessidades muito específicas 
- sum avg min max med 

![](https://github.com/luizrosalba/Arquitetura-de-Sistemas-Avan-ado.md/blob/master/Capturar.PNG?raw=true) 

-Em data warehouse tem como primeiro modelo sql 
- cubos de dimensoes : 
- tempo 
- membros 
- geografia 

- Olap dw : cubo de dimensoes consolidado dos dados mais utilizados 

## big data 
-Grande volume de dados estruturados, semi ou nao estuturados. 
- Formatos diversos de informações 
- não é um banco de dados nem uma grande ferramenta sozinha 
- trata de um grande volume de dados que juntas são utilizadas para extrair informações 
- dados estruturados 
são informações em formato padronizado solicitadas pelos mecanismos de busca para que eles possam entender o conteúdo das páginas web. 

- dados semi-estruturados 
estruturas de dados alteráveis sem a necessidade de uma  regra . obedecem uma estrutura basica mas podem ser alterados . NOSQL = Not Only sql 
apache hbase , cassandra , mongodb , riak , redis , 
Configurações de sistema xml , rdf , json , owl 
- alguns são baseados em chave valor , outros em wide column , document store , graph store ... 

- dados não estruturados
-hadoop , spark , presto , hdfs , apachestorm , datatorrent , google bigquery 
- haddop possui hdfs onde vc pode trazer qquer dado para hdfs 


## Data Lake vs Big Data

- Data lake é um grande conjunto de informações , um big date mais reservado, corporativo , tratado dentro de casa , no data lake temos entrada de daods estruturados , semi estruturados e não estruturados que são armazenados dentro de uma  empresa. ele precisa ter um sistema de data curation , quanto tempo ele fica como ele vai ficar. 

- mostrou como instalar o mongoDB

- jamais deletar ou usar  os Dbs admin , config e local 
- use loja (cria o db loja caso nao exista ) 
- db.produtos.insert({codigo:"01", descricao:"caneta"})  (cria uma nova tabela produtos) 
- db.produtos.find()  (retorna um id com um valor)
-ele é semistruturado , (não há necessidade de alterar produtos para inserir um novo produto ) 
- db.produtos.insert({codigo:"01", descricao:"lapis",cor:"vermelha"})  (cria uma nova tabela produtos) 
- não precisei redefinir a esturura para que inserisse mais um componente cor
-gera uma grande facilidade de gerar , mas transfere a responsabilidade de controlar a estrutura para o sistema. 







