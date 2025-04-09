## PrjModeloRefinado
Repositório para o Desafio de Projeto DIO

### 📝 Descrição do Desafio
Este repositório foi criado como parte de um desafio de projeto. O objetivo é refinar um modelo conceitual.

O esquema do modelo foi adicionado ao repositório para análise e documentação. Este arquivo fornece o contexto necessário para compreender o esquema desenvolvido.

### 🎯 Objetivo do Projeto
O modelo inicial deve ser refinado com base nos seguintes requisitos:

- [x] Cliente PJ e PF Uma conta pode ser PJ ou PF, mas não pode ter as duas informações;

- [x] Pagamento: Pode ter cadastrado mais de uma forma de pagamento;

- [x] Entrega: Possui status e código de rastreio;


### 🛠️ Detalhamento dos Campos ENUM
Alguns campos do modelo utilizam o tipo ENUM para garantir consistência e limitar os valores permitidos. Abaixo estão listados os campos e suas respectivas opções:

**Tabela Terceiro - Vendedor**\
status_vendedor:
ENUM('ativo', 'inativo')

**Tabela Entrega**\
status_entrega:
ENUM('pendente', 'em trânsito', 'entregue')

**Tabela Pedido**\
status_pedido:
sql
ENUM('aberto', 'processando', 'finalizado', 'cancelado')

**Tabela Pagamento**\
tipo_pagamento:
ENUM('cartão de crédito', 'cartão de débito', 'boleto bancário', 'pix', 'dinheiro')\
status_pagamento:
ENUM('pendente', 'aprovado', 'recusado')
