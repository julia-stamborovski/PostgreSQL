# <img width="50" height="50" src="https://user-images.githubusercontent.com/87834766/235192658-9cc03c75-9b34-4330-97ec-46b0f8ee2f07.svg" /> PostgreSQL 
Este projeto de estudo utiliza o PostgreSQL como sistema gerenciador de banco de dados. Durante sua implementação, foram criadas estruturas de tabela utilizando a sintaxe CREATE TABLE para definir os campos e tipos de dados que seriam armazenados. Através da utilização da cláusula SELECT, foram realizadas consultas no banco de dados, obtendo resultados de acordo com as condições estabelecidas no comando WHERE.

Para adicionar dados ao banco de dados, foram utilizados comandos INSERT, permitindo a inserção de novas linhas na tabela. Através do comando UPDATE, também foi possível atualizar informações já existentes no banco de dados, enquanto o comando DELETE foi utilizado para remover dados indesejados.

Para filtrar registros de acordo com critérios específicos, foi utilizada a cláusula WHERE, que permite estabelecer condições de seleção, como valores específicos ou intervalos de valores. Além disso, a cláusula ORDER BY foi utilizada para ordenar os resultados de consultas de acordo com um ou mais campos específicos, enquanto a cláusula JOIN permitiu a junção de registros de diferentes tabelas, unindo informações relacionadas em uma única consulta.





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
