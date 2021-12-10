# docker
## Comando que baixa a imagem do Go dentro do container e sobe o container
```
docker-compose up -d 
```
## Comando para entrar no console do meu container Docker
```
docker exec -it aluno_app_1 bash
```
## Aparece os conteiners que estão rodando e os que rodaram
```
docker ps -a
```
## comando para mudar a porta para ser acessada direto na máquina 
```
docker run --name=nginx -p 8080:80 nginx
```
## Quando o container sair ele automaticamente é removido –rm
```
docker run --rm --name=nginx -p 8080:80 nginx
```
## Remover container
```
docker rm <nome do container>
```
## Comando para vincular pasta do computador com a pasta do container
```
docker run --rm --name=nginx -p 8080:80 -v pwd:/usr/share/nginx/html nginx
```
## Criando minha própria imagem usando docker file
```
docker build -t mariojorge/nginx-fc:latest .
```
## Comando para rodar servidor sem estar vinculado ao terminal -d
```
docker run --rm -d --name=nginx -p 8080:80 -v pwd:/usr/share/nginx/html nginx
```
## imagem criada
```
docker run --rm -p 8080:80 mariojorge/nginx-fc:latest
```
## subie imagem para dockerhub
```
docker push marioalbuquerque/nginx-fc
```
## Update programas dentro da imagem
```
apt update
apt install vim
```
## Pressione a tecla ESC e em seguida digite:
```
:q sai do vim
:q! sai do vim sem salvar
:wq grava as alterações realizas e sai
:x grava as alterações e sai
:qa para sair de todas as edições em curso
```
