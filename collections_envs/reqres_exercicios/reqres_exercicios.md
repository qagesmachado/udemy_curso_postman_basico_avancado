# Reqres Exercícios
Esta collection é destinada a criação do projeto de teste do conjunto de APIs do site [Reqres](https://reqres.in/api-docs/#/) e [Reqress Swagger](https://reqres.in/api-docs/#/).

## Importando Collection e Environment
- Crie um workspace ou utilize um já existente
- Arraste e solte os arquivos dessa pasta para dentro do seu Postman desktop.

## Exercícios
Foi preparado 5  exercícios básicos a serem feitos de alguns dos end-points. Para conseguir ter acesso a eles da forma mais fácil aconselho que importe o arquvio em json ou assista as aulas que será mencionado.

### 1 - GET {RESOURCE}
Esse teste fará uma busca em um conjunto de informações fictícias e não randômicas. O que permite quer façamos validações fixas. Valide:
- Status code 200
- valide os parâmetros "page" e "per page"

### 2 - GET USERS
Esse teste faz uma busca em um conjunto de informações de usuários e não randômicos. 

Faça uma requisição que tenha:
- page = 1
- per_page = 2

Dessa forma, será trazidos dois registros de usuários, valide:
- Status code 200
- E-mail de cada um dos dois usuários obtidos

### 3 - GET USER ID - EXIST
Esse teste faz uma busca em um conjunto de informações de um usuário em específico de acordo com o ID. 

Faça uma requisição que tenha:
- id = 1 ("/users/1")

Dessa forma, será trazidos 1 registro de um usuário específico, valide:
- Status code 200
- Valide as informaçõe dentro do atributo "data"

### 4 - GET USER ID - NON EXIST
Esse teste faz uma busca em um conjunto de informações de um usuário em específico de acordo com o ID, assim se colocarmos um ID que não existe obteremos um erro. 

Faça uma requisição que tenha um id não existente:
- id = 234 ("/users/234")

Dessa forma, não será trazidos nenhum registro, valide:
- Status code 404

### 5 - GET USER - DELAY
Esse teste faz uma busca em um conjunto de informações de usuário e coneguimento configurar manualmente um parâmetro de delay

Faça uma requisição que tenha delay configurado:
- delay=3 (/users?delay=3)

Valide:
- Status code 200
- Tempo de resposta: maior que ou menor que algum limiar

### 6 - REGISTER USER
Esse teste faz a criação de um usuário no banco. No entanto isso acontece de forma simulada/mockada. Será necessário utilizar um payload fixo como utilizado na collection importada ou copie o texto a seguir.

    {
        "email": "eve.holt@reqres.in",
        "password": "pistol"
    }

Valide que:
- id=4
- token não é vazio