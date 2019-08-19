# Teste Mobile Tradeup

## Desafio

O desafio é criar um sistema simples para pedir reembolsos. Esse sistema consiste em duas telas:

- uma listagem de reembolso, com opções para criar, editar e excluir reembolsos.
- uma tela de criação de reembolso.

### Pontuação

Será necessário para concluir o teste:

- O framework utilizado deverá ser obrigatoriamente React Native.
- Poderá ser utilizado qualquer biblioteca, Redux, Styled Components, Glamorous, React Navigation, etc.
- Deverá ser utilizado git para versionamento.
- A organização do código será avaliada.
- O uso de hooks, será um diferencial.
- O código deve funcionar em ambas as plataformas, Android e IOS.

### Prazo

Você tem 14 dias para a entrega do projeto a partir da data que o desafio foi enviado para você.

## Funcionalidades

### Listagem de reembolso

Na listagem, será necessário apenas bater na API e colocar os dados que forem enviados para serem mostrados na tela.
Nessa tela, será possível:

- Excluir um ou mais reembolsos.
- Editar um reembolso.
- Cadastrar um novo reembolso.

---

### Criação de reembolso

Na criação de reembolso, haverá um formulário com alguns campos que serão validados pela API:

- Nome completo
- CPF/CNPJ
- Cargo

Após os campos definidos do usuário, deverá ser possível adicionar os reembolsos:
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

Ao salvar, bater no endpoint com os dados dos reembolsos e mostrar um feedback para o usuário de **sucesso** ou **erro** do processo.

---

## Dados

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

## Entrega

- Desenvolva e versione esse projeto usando git e publique um repositório no GitHub.
- Crie um README com instruções claras sobre como executar seu projeto.
