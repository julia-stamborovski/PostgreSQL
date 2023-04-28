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
<small>Tabela com todos os tipos de dados mais comuns (SERIAL, VARCHAR, TEXT, CHAR, INTEGER, NUMERIC, BOOLEAN, DATE, TIME, TIMESTAMP) para aprender como cada um desses funcionam</small>

# INSERT INTO
~~~
INSERT INTO aluno(nome, cpf, observacao, idade, dinheiro, altura, ativo, data_nascimento,hora_aula, matriculado_em) VALUES ('Julia', '11111111110', 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla ac dui et nisl vestibulum consequat. Integer vitae magna egestas, finibus libero dapibus, maximus magna. Fusce suscipit mi ut dui vestibulum, non vehicula felis fringilla. Vestibulum eget massa blandit, viverra quam non, convallis libero. Morbi ut nunc ligula. Duis tristique purus augue, nec sodales sem scelerisque dignissim. Sed vel rutrum mi. Nunc accumsan magna quis tempus rhoncus. Duis volutpat nulla a aliquet feugiat. Vestibulum rhoncus mi diam, eu consectetur sapien eleifend in. Donec sed facilisis velit. Duis tempus finibus venenatis. Mauris neque nisl, pulvinar eu volutpat eu, laoreet in massa.', 19, 100.50, 1.81, TRUE, '2004-03-01', '17:30:00', '2023-04-27 16:16:05');
~~~

# SELECT * FROM - "id" como filtro
~~~
SELECT * FROM aluno WHERE id = 1;
~~~

# UPDATE
``` UPDATE nome_tabela  ``` -> <mark>Para atualizar a tabela.</mark> <br/>
``` SET  ``` -> <mark>Para informar os campos que modificaremos.</mark>

~~~
UPDATE aluno SET nome = 'shizuko', observacaso = 'nada', ativo = FALSE WHERE ID = 1;
~~~
![aviso](https://img.shields.io/badge/%3D%20-%20antes%20de%20atribuir%20um%20novo%20valor.-yellow)