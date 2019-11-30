# SQL Databases
## Introdução
**SQL** Atende por *Structured Query Language*, e é a linguagem mais usada para modelar, salvar e consultar Databases de tipo *relacional*.

## Databases Relacionais
São bancos de dados baseados na manipulação de tabelas, que por sua vez representam **entidades e/ou relações entre entidades**.
## Iniciando em SQL
Existem certas ações que serão executadas muitas vezes durante o aprendizado, como, por exemplo, criar um novo database, utilizar um database já existente, inserir entidades nele, e assim por diante.

A intenção desse capítulo é justamente concentrar esses comandos básicos, para que esse arquivo também sirva de consulta:

    CREATE DATABASE <database_name>;
    
    USE <database_name>;
    
    CREATE TABLE <table_name> (
	    <attribute_name> TYPE(),
	    <attribute_name2> TYPE()
	); 
	
	INSERT INTO <table_name> (attribute_name, attribute_name2) 
		VALUES ('foo', 300);
		
	SELECT * FROM <table_name>;

 - A 1ª query  serve para criar um database no servidor mysql local;
 - A 2ª query serve para utilizar um database criado anteriormente;
 - A 3ª query serve para criar uma tabela no database escolhido;
 - A 4ª query serve para inserir uma entidade(**row**) nessa tabela.
 - A 5ª query serve para retornar todas as entidades que populam a referida tabela.
 
 **OBS**.: O asterisco na query `SELECT * FROM <table_name>;` se refere às colunas que deverão ser selecionadas da entidade, logo, caso esse (*) seja trocado pelo nome das colunas desejadas, elas serão recuperadas na ordem desejada pelo usuário(`SELECT column_1 FROM <table_name>`).
## Cláusula SELECT
A cláusula **SELECT** é utilizada para recuperar entidades de uma tabela, como já visto, porém, há mais detalhes nesse processo do que se imagina.
### Função do WHERE
O papel da cláusula **WHERE** associada à cláusula **SELECT** é importantíssima, dada a necessidade de filtrar uma busca na base de dados.

Esse termo pode filtrar de acordo com igualdades, desigualdades, casamento de padrões(**LIKE**), e assim por diante, podendo serem associadas várias condições juntas, o que permite das buscas muito gerais, até as mais específicas.

    SELECT column_1, column_2 FROM <table_name> 
	    WHERE column_1>column_2;

Esse código retorna as colunas 1 e 2 dos itens pertencentes a uma tabela que obedecem a desigualdade especificada no WHERE.

Operações também podem ser introduzids como colunas em um requisição SELECT, como por exemplo:

    SELECT column_1, column_2, CONCAT(column_1, ' e ',column_2) FROM <table_name>;
Esse SELECT retorna a coluna 1, a coluna 2 e a concatenação dessas duas na 3ª coluna de todas as linhas da referida tabela.

##

