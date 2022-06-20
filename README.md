# Docker e Digital Ocean

Desafios superados utilizando docker e digital ocean. Foi utilizado Droplets, Apps, Banco de dados entre outras coisas 

## Comandos uteis docker

**Login no docker Hub:** 
```bash 
docker login 
```

**Informações sobre os containers locais:** 
```bash 
docker ps -a 
```

**Listar imagens docker locais:** 
```bash 
docker images 
```

**Remover uma imagem do docker local:**  docker rmi -f < image>
**Ex:** docker rmi -f allefsousa/mymiles:0.0.0.4 
```bash 
docker rmi -f allefsousa/mymiles:0.0.0.4 
```

**Construir imagem docker:** docker build . (rodar no diretorio que estiver o docker file)   
```bash 
docker build .
```

**Renomear imagem apos geração:**  docker build -t < image_name>   .   
**Ex**: docker build -t allefsousa/mymiles:0.0.4 . 
```bash 
docker build -t allefsousa/mymiles:0.0.4 .
```

**Executar a imagem na maquina local:** docker run -p < porta> < image>   
**Ex:** docker run -p 8080  allefsousa/mymiles:0.0.4  
```bash 
docker run -p 8080  allefsousa/mymiles:0.0.4 
```

**Descobri IP do container local:** docker inspect < CONTAINER ID> | grep "IPAddress"
```bash 
docker inspect < CONTAINER ID> | grep "IPAddress"
```

## Links uteis
[Deploy spring boot in droplet](https://www.digitalocean.com/community/questions/deploy-spring-boot-jar-fie)

[Usar Screen no ubuntu para deixar a aplicação rodando](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-screen-on-an-ubuntu-cloud-server)

[Criando meu primeiro dockerfile](https://www.youtube.com/watch?v=5QGexrfqu60)

[Repositorio no dockerhub](https://hub.docker.com/repositories)

[Subindo uma imagem para o dockerhub](https://jtemporal.com/subindo-imagens-docker-pro-dockerhub/)

[Github Action deploy springboot in github artfacts](https://www.youtube.com/watch?v=a27v_VDD-eA)

[Repositorio base para criar o dockerfile do my miles](https://github.com/mcicolella/docker-microservice)

## Primeiro dockerfile 

<script src="https://gist.github.com/allefsousa/df180b874deb363933807cc5fc78e00f.js"></script>
