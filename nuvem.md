# Fundamentos de arquitetura de aplicações em nuvem
cloud computing 
- gerenciamento de hardware / software 
= provedores de servidor e armazenamento 
- pague o que consumir 
- Iaas / Paas / Baas 

 Infrastructure as a service  (Iaas) 
 - google cloud 
 - amazon web services 
 - microsoft azure 
 Plataform as a service (Paas) 
 - Máquinas e escalar máquinas , 
 - escreva a infra como código com sintaxe terraform e consegue prover todas as maquinas necessarias 
 - terraform 
 - amazon cloud formation 
 - facilidade de tracking, rollback e versionamento 
 
 Backend as a service (Baas) 
 - Mobile backend as a service 
  - autenticação 
  - Firebase , permite focar na aplicação , lida com dados e autenticação 
 
 ![](https://github.com/luizrosalba/Arquitetura-de-Sistemas-Avan-ado.md/blob/master/Capturar1221.PNG?raw=true) 
 
 ## Entenda sobre disponibilidade de aplicações
 Iaas 
 - nao precisamos nos preocupar com infraestrutura
 Paas 
 - auto scale on the go
 Baas 
 - não há backend service 
 
 Disponibilidade do app ou serviço 
 - as empresas estao utilizando docker para facilitar o desenvolvimento 
 - Kubernets (k8s) plugin que lida com api para distribuir os servicos pelos nodos  
 - multiplos nodos (minimo 3 workers kubernets e 3 instancias , 1 instancia em cada nodo , se um dá problema os outros assumem) 
 - load balancer ( utilizar os nodos de maneira igual ) 
 
 
 ## Aprenda a executar serviços com Serveless 
 
 - sem servidor 
 - sem serviço rodando 
 - sem down time 
 - o provedor garante que vc nao precisa cuuidar do servidor que ele prove para você  
 
 - api gateway 
 - amazon kinesis
 - aws lambda 
 - amazon s3 
 
 - lambda function - lida com eventos e seu código sera invocado 
 - o provedor garante o recebimento do request 
 
 -desvantagem: 
 - custo maior 
 - grande numero de lambdas (execuções pesadas são interrompidas pela aws ) 
 
 
 
 
 
