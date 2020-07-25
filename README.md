# 01# Docker

## Passos de como instalar o Docker no Ubuntu

#### 1. Atualize seu Sistema
    - Então, o sistema precisa ser atualizado para você ter mais segurança e
      confiabilidade para a instalação do Docker. Execute os dois comandos abaixo:

        - $ sudo apt update
        - $ sudo apt upgrade


#### 3. Instale Pacotes Pré-requisitos
    
    - Assim que atualizar o sistema, você deve instalar alguns dos pacotes 
      necessários antes de instalar o Docker Ubuntu. Você pode fazer isso com
      a ajuda de um único comando:

         $ sudo apt-get install  curl apt-transport-https ca-certificates software-properties-common


#### 4. Adicione os Repositórios do Docker

    - Agora você tem adicionar os repositórios do Docker.
      Isso vai fazer com que o processo de instalação seja
      muito mais fácil. Isso habilita você a usar o método oficial suportado de instalação.

    - Primeiro, você adiciona uma chave GPG, inserindo o comando a seguir na linha de comando do sistema:

          $ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -


#### 5. Agora, adicione o repositório executando este comando:
     
     $ sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
    
     - Depois disso, apenas atualize a informação do repositório

          $ sudo apt update


#### 6. Instalar Docker Ubuntu 18.04
    - instalar o Docker no Ubuntu.

          $ sudo apt install docker-ce


#### 7. Verificar Status do Docker
    - Assim que a instalação estiver completa, é uma ótima ideia verificar o status do serviço.

          $ sudo systemctl status docker
