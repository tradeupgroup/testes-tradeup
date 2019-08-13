# Teste Front-end Tradeup

## Desafio
O desafio é criar um sistema simples para pedir reembolsos. Esse sistema consiste em duas páginas:
- uma listagem de reembolso
- uma página de criação de reembolso

### Pontuação
Será necessário para concluir o teste:
- Apenas código front-end será considerado no projeto (HTML, CSS, JavaScript).
- Frameworks CSS não serão permitidos. Todo código CSS deve ser escrito por você.
- Você pode utilizar pré-processadores CSS à vontade. 
- O projeto pode ser escrito em javascript puro ou utilizar frameworks como Vue.js, React ou outro.
- Gerenciadores de pacotes e task runners podem ser usados à vontade.
- O projeto precisa ser responsivo, funcionando tanto em desktop quando mobile.

### Prazo
Você tem 14 dias para a entrega do projeto a partir da data que o desafio foi enviado para você.

## Funcionalidades

### Criação de reembolso
Na criação de reembolso, haverá um formulário com alguns campos para serem aceitos:
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

---

### Listagem de reembolso
Na listagem, será necessário apenas bater na API e colocar os dados que forem enviados para serem mostrados na tela.
Nessa tela, será possível excluir os reembolsos.

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

### Entrega
- Desenvolva e versione esse projeto usando git e publique um repositório no GitHub.
- Crie um README com instruções claras sobre como executar seu projeto.
