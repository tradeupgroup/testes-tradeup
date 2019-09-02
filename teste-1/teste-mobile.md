# Teste Mobile Tradeup

## Objetivo

Neste teste, o seu objetivo é montar um sistema simples, onde será necessário
fazer um CRUD com autenticação e duas páginas que exibem os dados providos
de uma API Rest, fornecida por nós.

## Tecnologias

- React Native
- Git

Sinta-se livre para usar bibliotecas como Redux, Styled Components, Glamorous,
React Navigation, entre outros (se tiver alguma dúvida, pode perguntar também).

## Requisitos

Sinta-se livre para cumprir os requisitos da forma que julgar melhor, o
importante é que seja possível executar todas as ações descritas neles.

Você vai perceber que os requisitos são relativamente vagos, pois queremos ver
as suas escolhas e o que julga melhor para completar a tarefa.

- O APP consiste em três telas, sendo a primeira uma tela para o usuário efetuar
  login, e outras duas telas para o usuário autenticado, a segunda tela seria uma
  listagem de usuários cadastrados e a terceira tela, para ver os detalhes de um usuário.
- Não se preocupe com marcas, imagens bonitas, etc. O que será avaliado é a
  usabilidade, a qualidade do código e a eficiência.
- Para tela de Login:
  - Deve ser necessário fornecer email e senha para efetuar login
- Para listagem de usuários:
  - Para cada item do endpoint de usuários, deve ser exibido o nome, email e avatar.
  - Ao clicar em um item, deve-se ir para a página de detalhes do usuário
- Para detalhe do usuário
  - Devem ser exibidas as mesmas informações da listagem.

## Entregável

- Seu código deve estar funcionando em ambas as plataformas, Android e IOS.
- Repositório no Github com o seu código.
- O README do seu projeto deve conter:
  - Instruções para rodar o projeto, caso necessário.
  - Tecnologias usadas e a razão da escolha delas.

## Prazo

Você tem 7 dias para a entrega do projeto a partir da data que o desafio foi enviado para você.

## Dados

### Autenticação:

##### Request

POST [/api/login](https://reqres.in/api/login)

```js
{
    "email": "eve.holt@reqres.in",
    "password": "cityslicka"
}
```

##### Response

200

```js
{
    "token": "QpwL5tke4Pnpja7X4"
}
```

### Listagem de usuários:

##### Request

GET [/api/users?page=2](https://reqres.in/api/users?page=2)

##### Response

200

```js
{
    "page": 2,
    "per_page": 6,
    "total": 12,
    "total_pages": 2,
    "data": [
        {
            "id": 7,
            "email": "michael.lawson@reqres.in",
            "first_name": "Michael",
            "last_name": "Lawson",
            "avatar": "https://s3.amazonaws.com/uifaces/faces/twitter/follettkyle/128.jpg"
        },
        {
            "id": 8,
            "email": "lindsay.ferguson@reqres.in",
            "first_name": "Lindsay",
            "last_name": "Ferguson",
            "avatar": "https://s3.amazonaws.com/uifaces/faces/twitter/araa3185/128.jpg"
        },
        {
            "id": 9,
            "email": "tobias.funke@reqres.in",
            "first_name": "Tobias",
            "last_name": "Funke",
            "avatar": "https://s3.amazonaws.com/uifaces/faces/twitter/vivekprvr/128.jpg"
        },
        {
            "id": 10,
            "email": "byron.fields@reqres.in",
            "first_name": "Byron",
            "last_name": "Fields",
            "avatar": "https://s3.amazonaws.com/uifaces/faces/twitter/russoedu/128.jpg"
        },
        {
            "id": 11,
            "email": "george.edwards@reqres.in",
            "first_name": "George",
            "last_name": "Edwards",
            "avatar": "https://s3.amazonaws.com/uifaces/faces/twitter/mrmoiree/128.jpg"
        },
        {
            "id": 12,
            "email": "rachel.howell@reqres.in",
            "first_name": "Rachel",
            "last_name": "Howell",
            "avatar": "https://s3.amazonaws.com/uifaces/faces/twitter/hebertialmeida/128.jpg"
        }
    ]
}
```

### Listagem de usuários:

##### Request

GET [/api/users/2](https://reqres.in/api/users/2)

##### Response

200

```js
{
    "data": {
        "id": 2,
        "email": "janet.weaver@reqres.in",
        "first_name": "Janet",
        "last_name": "Weaver",
        "avatar": "https://s3.amazonaws.com/uifaces/faces/twitter/josephstein/128.jpg"
    }
}
```
