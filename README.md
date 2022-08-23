<img src="./docs/gary.jpeg" width="120"> 
# Stackspot Gary Mock Server
The purpose of this plugin is to create an environment where the developer can test his front end or other backend programs without having to have the services running in the staging environment or locally. With gary plugin you can test your applications locally without the need for real services.




## Requirements

#### 1)Install docker
https://docs.docker.com/desktop/install/windows-install/

#### 3)make sure docker is running and upload the mock server

#### 4) Install the stackspot

https://stackspot.com/

Go inside the stack project folder and type the command:
    
    $ cd onde-esta-minha-stack

install de plugin using stack command

    $ stk add plugin https://github.com/slackwarecps/plugin-gary-mock-server 


you can verify using the command on cli: 

    $ stk list plugin

    +------------------+---------------------------------------------------------+-----------------+
    | name             | description                                             | version(latest) |
    +------------------+---------------------------------------------------------+-----------------+
    | plugin-gary-mock | Adiciona uma pasta com um mock server para nao depender | no release      |
    |                  | de servidores online                                    |                 |
    +------------------+---------------------------------------------------------+-----------------+


### 5) Open a terminal and enter inside the folder and execute the docker-compose command

    $cd  plugin-gary-mock
    $ docker-compose up

### 6) Try the service endpoint and after it use postman ( it is a suggestion :P ) to Test

CURL command to import in POSTMAN

      curl --location --request GET 'localhost:1080/api/v1/quem-eh-o-batman' 



- Administration dashboard

  - http://localhost:1080/mockserver/dashboard

### 7)You can change the default api json file and create yourself api mock.

File: initializer.json


    [
      {
        "httpRequest": {
          "path": "/api/v1/cores"
        },
        "httpResponse": {
          "body":[
            {
                "id": 1,
                "nome": "Verde de Fome"
            },
            {
                "id": 4,
                "nome": "Vermelho apagado"
            },
            {
                "id": 26,
                "nome": "Azul Campinas"
            }
        ]
        }
      },

      {
        "httpRequest": {
          "path": "/api/v1/quem-eh-o-batman"
        },
        "httpResponse": {
          "body": "eh o Bruce wayne"
        }
      }

    ]

### 8) Use The Postman Collection to use Gary Mock Server

[Download Example Postman Collection]("./../docs/Gary%20Mock%20Server.postman_collection.json")






### Finally

be happy!


<img src="./docs/stick-ok.jpeg" width="200"> 


