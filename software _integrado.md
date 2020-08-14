# Desenvolvimento e operação de software integrado

DevOps 
Reune os trabalhos de : 
- Development 
- QA Quality Assurance 
- It Operations 

- Integram e automatizam os processos entre as equipes de desenvolvimento , operações e de apoio para a produção rapida e confiável de software 
- Criar uma cultura de colaboração entre as equipes 
- É uma mudança de mentalidade , uma cultura , um movimento , uma filosofia 

-## Framework CALMS 

-Culture , automation , lean , measurement , sharing 
- Cultura : As ferramentas de auotmação são inuteis se a area de desenolvimento e operações nao trabalharem juntas 
- Automatização : Elimina trabalho manual e repetitivo -> compilação teste , implementação e provisionamento 
- Lean: Entregas de valor ao cliente , objetivos e enxutos . Conhecer as limitações e gargalos do processo.  
- Mensuração : Tornar o feedback claro para os envolvidos. Os ciclos de desenvolviemnto são pequenos até a entrega regras de negócio . Criam conhecimento e previsibilidade sorbe possiveis incidentes. (logs, pesquisa) 
- Compartilhamento : Descentraliza o conhecimento evitando que os processos se tornem dependentes. Todo profissional deve conhecer todos os pontos (não até exaustãao mas noção)   

Os três caminhos : 
- Flow Elimina dispedicios gargalos demanda e entrega . Metodologias ágeis e automatização integração contínua ou entrega contínua 
Business -> Custumer 
- Dev -> Ops 
- Feedback  - Ciclos rápidos que visam resolver problemas o quanto antes. Monitoramento é a chave quegera informações relevantes 
Business -> Custumer -> Business 
- Learning - Aprendizado contínuo gera conhecimento através da experimentação. Hipóteses qsão melhores que uma certeza imediata. Trabalho dinâmico com times realizando experimentos em seu trabalho diário . Eliminar a cultura da culpa e aumente a colaboração 
Business -> Custumer -> Business -> Custumer -> Business -> Custumer -> Business 

## Entregando software 
## Planejamento : (plan) 
- Microsoft Teams 
- Draw.io 
- Balsamiq
- readmunk 
- Confluence 
- Jira 
## Codificação (code) 
-Visual studio 
- github
- sublime text 
- cmder
- git 
- Vscode 
- notepad++
## Construção (build) 
- Containerd
-docker 
-nuget
- npm 
- cri-o
- net cli 
- msbuild 
## teste (test) 
- unit.net
- leader.io
- apache jmeter
- selenium 
- runscope
- postman
- sonarqube
- code climate 
- codacy
## release 
- planejei codifiquei construi teste vou disponibizar 
## deploy (disponibilização - implantação em produção) 
- azure pipelines
- circleci 
- app veyor 
- gitlab ci 
- travis ci 
- jenkins 
- App veyor
## Operação (operate) implantação 
- kubernetes (orquestra containers) 
- rancher 
- microsoft azure 
- puppet 
- Terraform 
- Chef 
- OpenShift
- aws 

## Coletar metricas (telemetria) 
- datadog 
- prometheus 
- appmetrics 
- rollbar 
- zabbix 
- new relic 
- pushover 
- seq 
- monitis 


-  manual devops the devops handbook 


## continuous integration 

my app -> continuous delivery (aprove por mediador) 0> app deployed 
my app -> continuous deployment (sem aprove por mediador) 0> app deployed 
## deploy (disponibilização - implantação em produção) 
- azure pipelines
- circleci 
- app veyor 
- gitlab ci 
- travis ci 
- jenkins 
- App veyor

## pipelines
 
 ![](https://github.com/luizrosalba/Arquitetura-de-Sistemas-Avan-ado.md/blob/master/Capturarsdsadasd.PNG?raw=true)


Se trigger release é automatica - Continuous deployment 
Se trigger release precisa ser aprovada - Continuous delivery
- Pipeline do App Veyor 
 ![](https://github.com/luizrosalba/Arquitetura-de-Sistemas-Avan-ado.md/blob/master/Capturar22222.PNG?raw=true
)
- Ciclecy Pipeline 

![](https://github.com/luizrosalba/Arquitetura-de-Sistemas-Avan-ado.md/blob/master/circly.PNG?raw=true) 

- Configuração do yml de cada um 

![](https://github.com/luizrosalba/Arquitetura-de-Sistemas-Avan-ado.md/blob/master/aaaaaaa.PNG?raw=true)

- é importante colocar o build para mostrar que está buildando no proprio repositorio 

## Continuous inspection code quality 
Inspecionadores de qualidade que podem dizer se seu código está bom ou não 

-Identificar complexidade ciclomática. Quanto mais ramificações maior a complexidade. O codigo deve ser objetivo. 
- Complexidade cognitiva - dificuldade de entender seu código 
- código duplicado 
- vulnerabidade code smell ex : senha no codigo (expoem a senha)  método com 573 linhas 
- Padronização e estilos 
- TODO deixou algo incompleto pelo código 
- Débito técnico
- cobertura de testes com badges 
Ferramentas : 
- sonarqube 
- codeclimate
- codacy 

- Ferramentas de versionamento podem bloquear que as ferramentas de controle de qualidade vão para o release 



