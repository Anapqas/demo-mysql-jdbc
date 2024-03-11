# demo-mysql-jdbc
Demo de um CRUD utilizando jdbc e conexão com mysql
## Instalar MySQL com Ubuntu
1) Download do mysql server: <br />
  `sudo apt update`<br />
  `sudo apt install mysql-server`<br />
  `sudo mysql`<br />
    obs: se não conseguir acessar tente ->  `service mysql stop  && sudo service mysql start` <br />
    Dentro do mysql rode: <br />
   `ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY '[sua_senha]'`;
Após isso vai precissar de senha para entrar no my sql: `sudo mysql -uroot -p[sua_senha]` <br />
Configure usando : `sudo mysql_secure_installation`
2) Download do mysql workbench: <br />
Baixe o arquivo do site oficial, na sua versão do Ubuntu 
Execute com `sudo apt install ./[arquivo]`

Para acessar o workbench -> `mysql-workbench`

obs: para checar a versão do ubuntu -> `lsb_release -a`

## Abrir o projeto
1) Adicione o classpath do MySQL Connector/J no projeto.
2) Dentro do workbench rode o script para popular o banco -> https://github.com/acenelio/demo-dao-jdbc/blob/master/database.sql
3) Execute o programa.
