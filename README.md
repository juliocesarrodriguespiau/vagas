# CRUD PHP - POO, PDO e MySQL
CRUD com PHP orientado a objetos e MySQL.

Esse módulo de cadastro permite que sejam cadastrados oportunidades de vagas nas empresas.

## Bootstrap
Para deixar um pouco mais agradável a parte visual, foi utilizado o Bootstrap.

Você pode acessar e utilizar suas funcionalidades através do link: [https://getbootstrap.com/]
## Banco de dados - MySQL
No MySQL foi criado uma tabela da vagas_oportunidades conforme script abaixo:
```sql
  CREATE TABLE oportunidades_vagas (
  	id INT NOT NULL  AUTO_INCREMENT,
  	titulo VARCHAR(255),
  	descricao TEXT(65535),
  	ativo ENUM('S','N'),
  	data TIMESTAMP,
  	PRIMARY KEY (id)
  );
```

## Configurações DB
As credenciais do banco de dados estão no arquivo `./app/Db/Database.php` e devem ser alteradas de acordo com seu ambiente (HOST, NAME, USER e PASS).

## Composer
O gerenciador de dependências Composer foi utilizado na configuração do autoload das classes e possíveis dependências.

É necessário rodar o Composer para que tudo rode perfeitamente.

Caso não tenha o Composer instalado, baixe pelo site oficial: [https://getcomposer.org/download](https://getcomposer.org/download/)

Para rodar o composer, basta acessar a pasta do projeto e executar o comando abaixo em seu terminal:
```shell
 composer install
```

Será criada uma pasta `vendor` na raiz do projeto e você já poderá acessar pelo seu navegador.
