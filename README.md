# plugin-gary-mock-server
spotstack plugin-gary-mock-server

#Requisitos mínimos

#### 1)Instale o docker
https://docs.docker.com/desktop/install/windows-install/

#### 3)certifique-se que o docker esta rodando e suba o servidor de mock

#### 4) Instale o stackspot

entre dentro de uma stack
    
    $ cd onde-esta-minha-stack

e instale o plugin

    $ stk add plugin https://github.com/slackwarecps/plugin-gary-mock-server 

voce pode verificar usando o comando :

    $ stk list plugin

    +------------------+---------------------------------------------------------+-----------------+
    | name             | description                                             | version(latest) |
    +------------------+---------------------------------------------------------+-----------------+
    | plugin-gary-mock | Adiciona uma pasta com um mock server para nao depender | no release      |
    |                  | de servidores online                                    |                 |
    +------------------+---------------------------------------------------------+-----------------+


###5) entre na pasta e suba o docker-compose



