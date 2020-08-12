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
