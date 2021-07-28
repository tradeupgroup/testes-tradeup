# Back-end Test Trade UP

## Introdução

Este é um desafio para testar seus conhecimentos em Back-end PHP Laravel;

**O objetivo é avaliar a sua forma de estruturação e autonomia em decisões para construir algo escalável utilizando o laravel como framework.**

## Case

A empresa Pharma Inc, está trabalhando em um projeto em colaboração com sua base de clientes para facilitar a gestão e visualização da informação dos seus pacientes de maneira simples e objetiva em um Dashboard onde podem listar, filtrar e expandir os dados disponíveis.
O seu objetivo nesse projeto, é trabalhar no desenvolvimento da REST API da empresa Pharma Inc seguindo os requisitos propostos neste desafio.

## Recursos

1. Desenvolver REST API importando os dados do projeto: https://randomuser.me/documentation
2. Trabalhar em um repositório em seu github pessoal (não esqueça de colocar no readme a referência a este desafio).


## API

### Modelo de Dados:

Para a definição do modelo, consultar o endpoint [https://randomuser.me/api?results=1](https://randomuser.me/api?results=1) que foi consultado no Random Users trazendo um único resultado.

- `imported_t`: campo do tipo Date time com a dia e hora que foi importado;
- `status`: campo do tipo Enum com os possíveis valores draft, trash e published;

### Sistema do CRON

Para prosseguir com o desafio, precisaremos criar na API um sistema de atualização que vai importar os dados para a Base de Dados com a versão mais recente do [Random User](https://randomuser.me/documentation#format) uma vez ao dia. Adicionar aos arquivos de configuração o melhor horário para executar a importação (env).

A lista de arquivos do Random User, pode ser encontrada em:

- https://randomuser.me/api

Formato:
- JSON (default)

Ter em conta que:

- Todos os produtos deverão ter os campos personalizados `imported_t` e `status`.
- Importar os dados de maneira paginada para não sobrecargar a API do Random Users. Por exemplo, de 100 em 100 usuários.
- Limitar a importação a somente 2000 usuarios;


### A REST API


Na REST API teremos um CRUD com os seguintes endpoints:

- `GET /`: Retornar uma mensagem "Desafio REST Trade Up is Running"
- `PUT /users/:userId`: Será responsável por receber atualizações realizadas
- `DELETE /users/:userId`: Remover o usuario da base de dados
- `GET /users/:userId`: Obter a informação somente de um usuario da base de dados
- `GET /users`: Listar todos os usuários da base de dados

Obs: **Não esqueça de adicionar um [.gitignore](https://www.toptal.com/developers/gitignore)**

### Extras

- **Diferencial 1** Escrever Unit Test para os endpoints da REST API
- **Diferencial 2** Executar o projeto usando Docker
- **Diferencial 3** Escrever um esquema de segurança utilizando `API KEY` nos endpoints. Ref: https://learning.postman.com/docs/sending-requests/authorization/#api-key

## Readme do Repositório

- Deve conter o título do projeto
- Uma descrição sobre o projeto e uma frase
- Deve conter uma lista com linguagem, framework e/ou tecnologias usadas
- Como instalar e usar o projeto (instruções)
- Referenciar que é um desafio realizado para TradeUP.

## Prazo, Finalização e Instruções para Envio

Você tem **7 dias** para realizar o desenvolvimento e entrega do desafio.
Após esse prazo você deve entrar em contato com nossa equipe de RH e avisar sobre a finalização e enviar para correção.

- **Obs:** Enviar o repositório do github público.
