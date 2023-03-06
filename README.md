Docker utilização prática no cenário de Microsserviços
================================================================
Instrutor: [Denilson Bonatti](https://github.com/denilsonbonatti/)<br>
Desafio final do Bootcamp Linux do Zero da [Digital Innovation One](https://dio.me)

Muito se tem falado de containers e consequentemente do Docker no ambiente de desenvolvimento. Mas qual a real função de um container no cenários de microsserviços? Qual a real função e quais exemplos práticos podem ser aplicados no dia a dia? Essas são algumas das questões que serão abordadas de forma prática pelo Expert Instructor Denilson Bonatti nesta Live Coding. IMPORTANTE: Agora nossas Live Codings acontecerão no canal oficial da dio._ no YouTube. Então, já corre lá e ative o lembrete! Pré-requisitos: Conhecimentos básicos em Linux, Docker e AWS.


Este projeto é um exemplo de como utilizar o Docker Compose para criar um ambiente com um banco de dados MySQL e uma aplicação PHP.

Tecnologias Utilizadas
----------------------

*   Docker
*   MySQL
*   PHP
*   Nginx

Instalação
----------

Para utilizar este projeto, é necessário ter o Docker e o Docker Compose instalados na sua máquina.

1.  Clone este repositório na sua máquina:
    
    `wget https://github.com/exemplo/projeto-docker-compose.git`
    
2.  Na raiz do projeto, execute o seguinte comando:
    
    `docker-compose up -d`
    
    Esse comando irá iniciar os containers do MySQL, PHP e Nginx.

Utilização
----------

Acesse a aplicação PHP em seu navegador em [http://localhost:4500](http://localhost:4500).

O arquivo index.php contém um exemplo de conexão com o banco de dados MySQL e inserção de dados na tabela "clientes".

Para acessar o banco de dados, utilize as seguintes credenciais:

*   Host: localhost
*   Port: 3306
*   User: root
*   Password: db_password
*   Database: db_database

Arquivos
--------

*   `docker-compose.yml`: Arquivo de configuração do Docker Compose que define os serviços (MySQL, PHP e Nginx) e suas configurações.
*   `banco.sql`: Arquivo SQL contendo a criação da tabela "clientes".
*   `index.php`: Arquivo PHP com um exemplo de conexão com o banco de dados MySQL e inserção de dados na tabela "clientes".
*   `nginx.conf`: Arquivo de configuração do Nginx para o redirecionamento de tráfego para o serviço PHP.
