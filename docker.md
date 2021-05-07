# Hey! 👤

[![Github Badge](https://img.shields.io/badge/-Github-000?style=flat-square&logo=Github&logoColor=white&link=https://github.com/luciolemos)](https://github.com/luciolemos)
[![Linkedin Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/lucio-lemos-a550441a1/)](https://www.linkedin.com/in/lucio-lemos-a550441a1/)
[![Twitter Badge](https://img.shields.io/badge/-Twitter-1ca0f1?style=flat-square&labelColor=1ca0f1&logo=twitter&logoColor=white&link=https://twitter.com/lucciolemos)](https://twitter.com/lucciolemos)
[![Youtube Badge](https://img.shields.io/badge/-YouTube-ff0000?style=flat-square&labelColor=ff0000&logo=youtube&logoColor=white&link=https://studio.youtube.com/channel/UCrNM1nr2nw0lSqMD10m6rLw)](#)
## My Tips 📌:
### Docker CLI 💻
O [Docker](https://git-scm.com/) nada mais é que uma plataforma aberta para criação, execução e publicação (deploy) de containers. Um Container é a forma de empacotar sua aplicação e suas dependências (bibliotecas) de forma padronizada. Podemos dizer que as palavras chaves para o Docker são: construir, entregar e rodar em qualquer ambiente (develop, ship and run anywhere). Docker é uma plataforma aberta para desenvolvimento, envio e execução de aplicativos. O Docker permite que você separe seus aplicativos de sua infraestrutura para que possa entregar o software rapidamente. Com o Docker, você pode gerenciar sua infraestrutura da mesma forma que gerencia seus aplicativos. Tirando proveito das metodologias do Docker para enviar, testar e implantar código rapidamente, você pode reduzir significativamente o atraso entre escrever o código e executá-lo na produção.
#### ✔️ Verificando a versão do Docker instalada:
    luciolemos@Home:~$ docker -v
    Docker version 20.10.5, build 55c4c88

#### ✔️ Verificando o status dos serviços:
    luciolemos@Home:~$ service --status-all
    [ - ]  docker

#### ✔️ "Startando" o serviço do Docker:
    luciolemos@Home:~$ sudo service docker start
    * Starting Docker: docker  

#### ✔️ Verificando novamente o status dos serviços:
    luciolemos@Home:~$ service --status-all
    [ + ]  docker

#### ✔️ Verificando se a instalação do Docker foi bem sucedida:
    luciolemos@Home:~$ docker run hello-world
    Hello from Docker!
    This message shows that your installation appears to be working correctly.
    To generate this message, Docker took the following steps:
     1. The Docker client contacted the Docker daemon.
     2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
        (amd64)
     3. The Docker daemon created a new container from that image which runs the
        executable that produces the output you are currently reading.
     4. The Docker daemon streamed that output to the Docker client, which sent it
        to your terminal.
    To try something more ambitious, you can run an Ubuntu container with: $ docker run -it ubuntu bash
    Share images, automate workflows, and more with a free Docker ID: https://hub.docker.com/
    For more examples and ideas, visit: https://docs.docker.com/get-started/

#### ✔️ Pesquisando imagens disponíveis no Docher Hub (do ubuntu por exemplo). Na coluna "OFFICIAL", "OK", indica uma imagem construída e apoiada pela empresa mantenedora do Projeto Ubuntu, a Canonical. Depois de identificar a imagem que deseja usar, você pode baixá-la para o seu computador usando o subcomando "pull".
    luciolemos@Home:~$ docker search ubuntu
    NAME                                                      DESCRIPTION                                     STARS     OFFICIAL   AUTOMATED
    ubuntu                                                    Ubuntu is a Debian-based Linux operating sys…   12037     [OK]
    dorowu/ubuntu-desktop-lxde-vnc                            Docker image to provide HTML5 VNC interface …   515                  [OK]
    websphere-liberty                                         WebSphere Liberty multi-architecture images …   267       [OK]
    rastasheep/ubuntu-sshd                                    Dockerized SSH service, built on top of offi…   249                  [OK]
#### ✔️ Execute o comando a seguir, para baixar a imagem oficial do ubuntu:
    luciolemos@dev:~$ docker pull ubuntu
#### ✔️ Após o download de uma imagem, é possível executar um contêiner usando a imagem baixada com o subcomando "run". Como se viu, no exemplo do "hello-world", se uma imagem não tiver sido baixada, quando executada, o cliente Docker primeiro fará o download da imagem, para em seguida, executar um contêiner usando-a. Para visualizar quais imagens foram baixadas para o computador, use:
    luciolemos@dev:~$ docker images
    REPOSITORY    TAG       IMAGE ID       CREATED       SIZE
    ubuntu        latest    26b77e58432b   10 days ago   72.9MB
    hello-world   latest    d1165f221234   5 weeks ago   13.3kB
    
#### ✔️ Criando a imagem do container. O "docker build" cria nova imagem a partir do Dockerfile declarado.
    luciolemos@dev:~/my_docker_projects/app$ docker build -t getting-started .
    [+] Building 43.0s (11/11) FINISHED
     => [internal] load build definition from Dockerfile                                                                                                                   0.0s
     => => transferring dockerfile: 184B                                                                                                                                   0.0s
     => [internal] load .dockerignore                                                                                                                                      0.0s
     => => transferring context: 2B                                                                                                                                        0.0s
     => [internal] load metadata for docker.io/library/node:12-alpine                                                                                                     11.9s
     => [auth] library/node:pull token for registry-1.docker.io                                                                                                            0.0s
     => [internal] load build context                                                                                                                                      0.1s
     => => transferring context: 4.63MB                                                                                                                                    0.1s
     => [1/5] FROM docker.io/library/node:12-alpine@sha256:c4e50b1f0f4f86b7f1a2315efc9dea7e2d4152975da6125d1f981d8d0bca09b5                                                0.0s
     => CACHED [2/5] RUN apk add --no-cache python g++ make                                                                                                                0.0s
     => CACHED [3/5] WORKDIR /app                                                                                                                                          0.0s
     => [4/5] COPY . .                                                                                                                                                     0.0s
     => [5/5] RUN yarn install --production                                                                                                                               27.2s
     => exporting to image                                                                                                                                                 3.8s
     => => exporting layers                                                                                                                                                3.7s
     => => writing image sha256:918ddcb4d27edf3592407dca85db52ba749580410697b172c5412d7e9baddd8c                                                                           0.0s
     => => naming to docker.io/library/getting-started
    #### ✔️ Executando o container
    luciolemos@dev:~/my_docker_projects/app$ docker run -d -p 80:80 docker/getting-started
    Unable to find image 'docker/getting-started:latest' locally
    latest: Pulling from docker/getting-started
    ba3557a56b15: Pull complete
    468d8ccebf7a: Pull complete
    b7f67c5d6ce9: Pull complete
    ed91f01a4fcb: Pull complete
    8051568c89ac: Pull complete
    5b4dcb4d3646: Pull complete
    22ecfaabb4de: Pull complete
    bbaa3642d0a3: Pull complete
    Digest: sha256:67944b53f8a7d16b3d9909315f9d557ade12c4ee4083cd98068f9fe6d9995808
    Status: Downloaded newer image for docker/getting-started:latest
    52b57841101854c2e36169ab16fc7b88a23eb6fed109a08bee13058da218e37a
