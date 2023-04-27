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
<small>Tabela com todos os tipos de dados mais comuns (SERIAL, VARCHAR, TEXT, CHAR, INTEGER, NUMERIC, BOOLEAN, DATE, TIME, TIMESTAMP) para aprender como cada um desses funcionam.</small>
