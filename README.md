> # Asynchronous-Communication-With-Amazon-SQS
Projeto da disciplina de Sistemas Distribuidos

## 1. INTRODUÇÃO

A comunicação indireta via Amazon SQS é um modelo de troca de mensagens em sistemas distribuídos no qual os componentes não se comunicam diretamente entre si. Em vez disso, eles utilizam uma fila como intermediário para desacoplar produtores e consumidores.

### 1.1 Comunicação direta
Na comunicação direta:
- Um processo envia mensagem diretamente para outro.
- Em geral, ambos precisam estar ativos simultaneamente.
- Há maior acoplamento entre os serviços.

Exemplo:
`Serviço A faz uma requisição HTTP diretamente ao Serviço B.`

`A ----HTTP----> B`

Possui escalibidade mais dificil, A precisa conhecer o endereço de B. Além disso, se B cair, A falha.

### 1.2 Comunicação indireta
- O remetente envia mensagens para um intermediário.
- O destinatário lê quando puder.
- Os serviços ficam desacoplados.

`Serviço A ---> Amazon SQS ---> Serviço B`

## 2. ETAPAS
- [ ]  Ter uma base teórica do assunto: fundamentos de SQS e de como usar o respectivo serviço da Amazon AWS.
- [ ]  Arquitetura básica do sistema (OK)
- [ ]  Aplicações já prontas que usem de SQS.
- [ ]  Implementar num sistema com um objetivo específico.
