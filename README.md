# Teste Front-end Tradeup

## Desafio
O desafio é fazer uma tela simples de pedido de reembolso.
A tela consiste em um formulário com alguns campos para serem aceitos:
- Nome completo
- CPF/CNPJ
- Cargo

Após os campos definidos dos usuários, deverá ser possível adicionar os reembolsos:
Limite de no máximo 15 reembolsos por vez.
Também deverá ser possível remover cada reembolso.
No reembolso deverá ter:
- Data
- Tipos de Reembolso
```
Passagem/Hospedagem - ID: TICKET
Alimentação - ID: FOOD
Telef. / Lavanderia - ID: TEL
Transporte - ID: TRANS
Estacionament/Pedágio - ID: PARKING
Outras despesas - ID: OTHER
```
- Descrição do reembolso
- Valor do reembolso

Ao salvar, bater no endpoint com  os dados dos reembolsos e mostrar um **modal** com o **sucesso** ou **erro** do processo.

Os dados do reembolso devem ser enviados da seguinte maneira:
```js
{
  name: 'Gabriel Josefino',
  identification: '00000000000',
  jobRole: 'Não sei',
  refunds: [
    {
      date: '2019-08-12T09:33:20-03:00',
      type: 'TICKET',
      description: 'Gastei com a passagem para Porto Alegre'
      value: 108.90
    }
  ]
}
```
