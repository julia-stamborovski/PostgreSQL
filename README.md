# PostgreSQL

## Versão
12.9

- Criação de estruturas de uma tabela com CREATE TABLE
- Realização de consultas com SELECT
- Adiconar dados no banco com INSERT
- Atualizar e apagar dados com UPDATE e DELETE
- Filtrar os registros com WHERE
- Ordernar os dados com o ORDER BY
- Juntar os registros de tabelas com JOIN

# Criação de banco de dados
~~~
CREATE DATABASE alura;
~~~

Comando 
~~~
\l
~~~
<small>Para visualizar os bancos de dados</small>

# Exclusão de banco de dados
~~~
DROP DATABASE alura;
~~~

# Criação de tabela 
~~~
CREATE TABLE aluno( id SERIAL, nome VARCHAR(255), cpf CHAR(11), observacao TEXT, idade INTEGER, dinheiro NUMERIC(10,2), altura REAL, ativo BOOLEAN, data_nascimento DATE, hora_aula TIME, matriculado_em TIMESTAMP);
~~~
<<<<<<< HEAD
<small>Tabela com todos os tipos de dados mais comuns (SERIAL, VARCHAR, TEXT, CHAR, INTEGER, NUMERIC, BOOLEAN, DATE, TIME, TIMESTAMP) para aprender como cada um desses funcionam</small>

# INSERT INTO
~~~
INSERT INTO nome_tabela_aqui [ ( colunas [, ...] ) ]
    { DEFAULT VALUES | VALUES ( { expression | DEFAULT } [, ...] ) | query }
~~~
=======
<small>Tabela com todos os tipos de dados mais comuns (SERIAL, VARCHAR, TEXT, CHAR, INTEGER, NUMERIC, BOOLEAN, DATE, TIME, TIMESTAMP) para aprender como cada um desses funcionam.</small>
>>>>>>> d3a75631ab12b58bd3ae86a9e7a6f54def22a6d5
