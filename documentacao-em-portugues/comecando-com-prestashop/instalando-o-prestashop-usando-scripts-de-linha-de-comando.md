# Instalando o PrestaShop usando scripts de linha de comando

## Instalando o PrestaShop usando scripts de linha de comando <a href="#instalandooprestashopusandoscriptsdelinhadecomando-instalandooprestashopusandoscriptsdelinhadecomand" id="instalandooprestashopusandoscriptsdelinhadecomando-instalandooprestashopusandoscriptsdelinhadecomand"></a>

Desde a versão 1.5.4, o PrestaShop possui script de linha de comando para fazer a instalação.

### O que é isto? <a href="#instalandooprestashopusandoscriptsdelinhadecomando-oqueeisto" id="instalandooprestashopusandoscriptsdelinhadecomando-oqueeisto"></a>

Este instalador faz com que seja possível instalar o PrestaShop sem a necessidade de usar um navegador web: basta colocar o conteúdo do arquivo zip em seu servidor web, e você pode instalar o PrestaShop através da interface de linha de comando (CLI). Qualquer software de linha de comando pode ser usado, desde que você pode usá-lo para interagir com comandos do servidor: Bash, Windows PowerShell, OS X Terminal, PuTTY, etc.

O fator principal de se ter um instalador por linha de comando, além do instalador regular no navegador é dar essa opção para atender a alguns usuários avançados, que muitas vezes preferem interfaces de linha de comando, pois eles tendem a proporcionar um meio mais conciso e poderoso para controlar um programa ou sistema operacional.

### Como usar? <a href="#instalandooprestashopusandoscriptsdelinhadecomando-comousar" id="instalandooprestashopusandoscriptsdelinhadecomando-comousar"></a>

O instalador de linha de comando é fácil de usar: a partir de seu terminal, vá para a pasta / instale (ou / install-dev)  e inicie o script com este comando:

```
$ php index_cli.php
```

Isto irá mostrar todas as opções disponíveis.

![](<../../.gitbook/assets/16779385 (1).png>)

Todas as opções do instalador regular no navegador estão disponíveis com o seu valor padrão. Quase todos os valores padrões podem ser deixado como estão, pois você pode editar todos a partir do painel administrativo do PrestaShop uma vez que a instalação estiver terminada. Note que o e-mail e senha serão aqueles usados para criar a conta do painel de administração...

Para iniciar a instalação, você só precisa fornecer um argumento. Na realidade, você precisa fornecer:

* **domain**. O dominio onde você quer que sua loja para aparecer.
* **db\_server**. O endereço do servidor de banco de dados.
* **db\_name**. O nome do banco de dados que deseja usar.
* **db\_user**. O nome de usuário do banco de dados que deseja usar.
* **db\_password**. A senha para o nome de usuário de banco de dados acima.

Por exemplo:

```
$ php index_cli.php --domain=examplo.com --db_server=sql.examplo.com --db_name=prestashop --db_user=root --db_password=123456789
```

![](<../../.gitbook/assets/16779386 (1).png>)

Se você também definir o valor --email para o seu endereço, um e-mail de confirmação será enviado a você uma vez que a instalação estiver finalizada.

### Lista de argumentos <a href="#instalandooprestashopusandoscriptsdelinhadecomando-listadeargumentos" id="instalandooprestashopusandoscriptsdelinhadecomando-listadeargumentos"></a>

Aqui está a lista de argumentos para o index\_cli.php da versão 1.6:

| Nome           | Valor Padrão                                    | Descrição                                               |
| -------------- | ----------------------------------------------- | ------------------------------------------------------- |
| --step         | process                                         |                                                         |
| --language     | en                                              | Código ISO do Idioma                                    |
| --timezone     | localhost                                       |                                                         |
| --domain       | localhost                                       |                                                         |
| --db\_server   | localhost                                       |                                                         |
| --db\_user     | root                                            |                                                         |
| --db\_password | (blank)                                         |                                                         |
| --db\_name     | prestashop                                      |                                                         |
| --db\_clear    | 1 (true)                                        | Apaga tabelas existentes                                |
| --db\_create   | 0 (false)                                       | Criar o banco de dados se ele não existir               |
| --prefix       | ps\_                                            |                                                         |
| --engine       | InnoDB                                          | InnoDB/MyISAM                                           |
| --name         | PrestaShop                                      | Nome da loja                                            |
| --activity     | 0                                               |                                                         |
| --country      | fr                                              |                                                         |
| --firstname    | John                                            |                                                         |
| --lastname     | Doe                                             |                                                         |
| --password     | 0123456789                                      |                                                         |
| --email        | [pub@prestashop.com](mailto:pub@prestashop.com) |                                                         |
| --license      | 0 (false)                                       | Mostrar a licença do PrestaShop                         |
| --newsletter   | 1 (true)                                        | Subscrever o administrador na newsletter do PrestaShop  |
| --send\_email  | 1 (true)                                        | Enviar um e-mail para o administrador após a instalação |
