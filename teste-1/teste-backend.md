# Teste Back-end Tradeup

## Desafio
O desafio é criar um sistema simples para pedir reembolsos. Esse sistema consiste em duas páginas:
- uma listagem de reembolso
- uma página de criação de reembolso


## Pontuacao

Para o teste ser considerado precisa atender aos requisitos minimos será analisado

- organizacao do código
- uso dos verbos HTTP
- boas práticas de API Rest


## Tecnologias

Banco de dados: MySQL ou MongoDB
Linguagem: PHP
Framework: Laravel
Framework de teste: PHPUnit
API: Rest

## Funcionalidades

### Cadastro de reembolso

Implementar um serviço que receba os dados do reembolso e persista no banco de dados:

```js
{
  name: 'Gabriel Josefino',
  identification: '00000000000',
  jobRole: 'Não sei',
  refunds: [
    {
      date: 2019-08-12T09:33:20-03:00',
      type: 'TICKET',
      description: 'Gastei com a passagem para Porto Alegre'
      value: 108.90
    }
  ],
  createdAt : '2019-08-12T09:33:20-03:00'
}
```

---
### Edicao de reembolso

A edicao de desconto deve permitir apenas a alteracao do valor

---

### Listagem de reembolso
A listagem deve conter todos os dados previamente cadastrados e páginados de 10 em 10 itens por página.

---

### Relatório

A API deve ser capaz de através de paremtros enviados na requisicao gerar um relatório do valor total de reembolsos por usuário e por mes.

```js
{
  month: 9,
  year: 2019,
}
```


