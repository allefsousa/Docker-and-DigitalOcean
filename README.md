# Docker e Digital Ocean

Desafios superados utilizando docker e digital ocean. Foi utilizado Droplets, Apps, Banco de dados entre outras coisas 

# Comandos uteis docker

**Login no docker Hub:** docker login 

**Informações sobre os containers locais:** docker ps -a

**Listar imagens docker locais:** docker images 

**Remover uma imagem do docker local:**  docker rmi -f < image>
**Ex:** docker rmi -f allefsousa/mymiles:0.0.0.4 

**Construir imagem docker:** docker build . (rodar no diretorio que estiver o docker file)   

**Renomear imagem apos geração:**  docker build -t < image_name>   .   
**Ex**: docker build -t allefsousa/mymiles:0.0.4 .  

**Executar a imagem na maquina local:** docker run -p < porta> < image>   
**Ex:** docker run -p 8080  allefsousa/mymiles:0.0.4   

**Descobri IP do container local:** docker inspect < CONTAINER ID> | grep "IPAddress"
