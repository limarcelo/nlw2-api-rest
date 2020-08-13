# FUNCIONALIDADES

## Conexoes
- Rota para criar uma conexao aluno/professor;
- Rota para listar o total de conexões realizadas;

## Aulas
- Rota para criar aula;
- Rota para listar aulas;
    - Filtrar por matéria, dia da semana e horário;


## Configurações para criacao do projeto
- yarn init -y
- yarn add typescript -D
- yarn tsc --init //alterar arquivo tsconfig.son  "target": "es2017";
- yarn add ts-node-dev -D
- yarn add express
- yarn add @types/express -D
- yarn add knex sqlite3

# configuracao do package.json
"scripts": {
    "start": "tsnd --transpile-only --ignore-watch node_modules --respawn src/server.ts",
    "knex:migrate": "knex --knexfile knexfile.ts migrate:latest",
    "knex:migrate:rollback": "knex --knexfile knexfile.ts migrate:rollback"
},