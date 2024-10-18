# MovieFlix API

MovieFlix API é um serviço backend projetado para gerenciar e fornecer acesso a um banco de dados de filmes. Ele serve como o núcleo para dados relacionados a filmes, como títulos, gêneros, idioma, classificações e avaliações.

Este projeto é desenvolvido com Node.js, Express e Prisma ORM para o gerenciamento do banco de dados, oferecendo uma API RESTful que pode ser integrada com um frontend ou aplicativo mobile para proporcionar uma experiência perfeita de navegação por filmes.

## Funcionalidades

- Gerenciamento de Dados de Filmes: Adicionar, atualizar e deletar filmes e séries.
- Classificação por Gênero: Filtrar filmes por gênero.
- Funcionalidade de Pesquisa: Buscar filmes por título, gênero ou ano.
- Gerenciamento de Banco de Dados com Prisma: Utiliza o Prisma ORM para interações eficientes com o banco de dados.

## Stack Tecnológico

- Node.js: Ambiente de execução JavaScript.
- Express.js: Framework web rápido e minimalista.
- Prisma ORM: ORM de última geração para gerenciamento de banco de dados.
- PostgreSQL/MySQL: Banco de dados backend (escolher com base na configuração).
- ESLint & Prettier: Para linting e formatação de código.

## Instalação

1. Clone o repositório:

    ```bash
        git clone https://github.com/Rafaela-Wolf/movieflix-api.git
        cd movieflix-api

2. Instale as dependências:

    ```bash
        npm install

3. Configure suas variáveis de ambiente:

    Crie um arquivo .env no diretório raiz e configure com suas credenciais do banco de dados e outras variáveis necessárias. Aqui está um exemplo:

    ```env
        DATABASE_URL=postgresql://usuario:senha@localhost:5432/movieflix

4. Execute as migrações do banco de dados:

    ```bash
        npx prisma migrate dev

5. Inicie o servidor:

    ```bash
        npm run dev

6. O servidor estará rodando em http://localhost:3000.

## Endpoints da API

Aqui estão alguns dos principais endpoints disponíveis na MovieFlix API:

### Filmes

- GET /movies: Obter uma lista de todos os filmes.
- GET /movies/: Obter detalhes de um filme específico.
- POST /movies: Adicionar um novo filme (somente Admin).
- PUT /movies/: Atualizar um filme (somente Admin).
- DELETE /movies/: Deletar um filme (somente Admin).

## Modelo de Banco de Dados

O esquema do banco de dados é gerenciado com o Prisma e inclui tabelas para:

- Filmes: Armazena informações sobre filmes e séries de TV.
- Gêneros: Classifica filmes em gêneros.

Para visualizar ou modificar o esquema, confira o arquivo prisma/schema.prisma.

## Contribuição

Se você deseja contribuir para este projeto:

1. Faça um fork do repositório.
2. Crie uma nova branch com sua feature ou correção de bug.
3. Envie um pull request com as alterações detalhadas.