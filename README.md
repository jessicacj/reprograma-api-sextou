# {reprograma} Semana 10 - NODE.JS + MONGO + API :computer:

![rep](https://user-images.githubusercontent.com/42447794/69483022-3549b300-0e01-11ea-85f0-a8de16f95179.png)

## API de Catálogos de Filmes

Elaboração de uma **API** de Catálogo de Filmes com **Node.JS** e **MongoDB**.

### Objetivo

Criar uma API, com banco de dados, que retorne qual filme deve aparecer no topo da lista de sugestões do catálogo.

#### Requisitos:

- [x] Cada filme deve possuir os seguintes campos: nome, ano, avaliações, quantidade de exibições;
- [x] Não podemos ter filmes diferentes com o mesmo nome;
- [x] Avaliações é uma lista de números, em que cada número representa a avaliação da pessoa de 1 a 5 (estrelas). Exemplo: {avaliacoes: [2,3,1,4,5,5,1,2]};
- [x] A pontuação do filme é calculada multiplicando a média de avaliações com a quantidade de exibições. 

### Ferramentas utilizadas

### Instalação

### Endpoints

- GET "/" => rota inicial da API.
- GET "/filmes/catalogo" => retorna os filmes ordenados por pontuação, exibindo a pontuação de cada filme.
- POST "/filmes/criar" => recebe um novo filme, com parâmetros de nome e ano, para ser adicionado ao banco de dados.
- PATCH "/filmes/exibicao/:id" => adiciona +1 na quantidade de exibições e pode receber no body uma avaliação (opcional) a ser adicionada na lista de avaliações.
- DELETE "/filmes/remover/:id" => remove o filme do catálogo pelo ID.

