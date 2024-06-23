# Faker API Exercícios
Esta collection é destinada a resolução exercícios de fixação envolvendo as APIs do site [Faker API](https://fakerapi.it/en).

## Importando Collection e Environment
- Crie um workspace ou utilize um já existente
- Arraste e solte os arquivos dessa pasta para dentro do seu Postman desktop.

## Collections

### Address
Pergunta 1 - Fazer uma requisição no endpoint "/address" que:

    - Busque 1 endereço
    - Utilize parâmetro “seed”
    - Valide o status code
    - Valide a quantidade de endereços buscados
    - Valide que os campos gerados serão sempre os mesmos

### Books
Pergunta 1: Fazer uma requisição no endpoint "/books" que:
    
    - Busque 5 livros
    - Valide que foram buscados 5 livros sem utilizar o campo “total” do response body

### Companies
Pergunta 1: Fazer uma requisição no endpoint "/companies" que:

    - Busque 1 elemento
    - Capture quantos endereços esse elemento companhia possui e salve em uma variável
    - Imprima no console o valor dessa variável

### Credit Cards
Pergunta 1: Fazer uma requisição no endpoint "/credit_cards" que:
    
    - Busque 3 elementos
    - Utilize uma lista de possíveis resultado pra verificar se um deles é igual ao campo type
    - Crie uma lista que não tenha resultados certos e faça um teste negativo

### Images
Pergunta 1: Fazer uma requisição no endpoint "/images" que:

    - Busque 1 elemento
    - Elemento deve ter _width e _height configurado
    - Valide que obteve-se o valor certo de _width e _height 

Pergunta 2: Fazer uma requisição no endpoint "/images" que:

    - Mude alguns dados de forma randômica: _width, _height, Tamanho da imagem, Tipo da imagem
    - Os parâmetros definidos de forma randômica devem ser criados no pre-request script
    - Valide-os no POST-Response
    - Será necessário parametrizar a URL de requisição com os dados randômicos
    - Observe que o tipo de imagem "kittens" gera variações na url, será necessário implementar um condicional "if"

### Persons
Pergunta 1: Fazer uma requisição no endpoint "/persons" que:

    - Utilize _quantity = 1
    - Utilize os parâmetros: _gender, _birthday_start , _birthday_end
    - Valide o gênero escolhido (se desejar pode fazer de forma randômica)
    - Valide as datas escolhida

Pergunta 2: Fazer uma requisição no endpoint "/persons" que: 

    - Utilize _quantity > 1
    - Utilize os parâmetros: _gender, _birthday_start , _birthday_end
    - Valide o gênero escolhido (se desejar pode fazer de forma randômica)
    - Valide as datas escolhida

Pergunta 3: Fazer uma requisição no endpoint "/persons" que:

    - Utilize gender fixo
    - Utilize o parametro "seed"
    - Utilize a função com .find() para encontrar algum Firstname e validar se existe
    - Utilize a função com .find() para validar que não existe um dos generos
    Gender

### Places
Pergunta 1: Fazer uma requisição no endpoint "/places" que:

    - Valide quais hemisférios está o endereço gerado utilizando Latitude e Longitude

### Products
Pergunta 1: Fazer uma requisição no endpoint "/products" que:

    - Valide que preços min e max estão dentro do range pedido
    - Valide o preço antes e após taxas
