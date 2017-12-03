# Fullstack - 0.1-SNAPSHOT

Este projeto tem a intenção de servir de exemplo em como subir um
todos os serviços e servidores mais comuns durante o desenvolvimento de uma
aplicação fullstack (backend + frontend), utilizando containers do docker.

## Serviços:
* Servidor Web Nginx
* Servidor de Aplicação Wildfly
* Banco de dados PostgreSQL
* E outros mais que forem interessantes

## Dependências:
* (Docker)[https://www.docker.com/] - Instruções de instalação (aqui)[https://docs.docker.com/engine/installation/]
* (Docker Compose)[https://docs.docker.com/compose/] - Instruções de instalação (aqui)[https://docs.docker.com/compose/install/]


## Estrutura do Projeto:

Neste projeto, cada serviço possui o seu próprio diretório, contendo mais
informações a cerca de suas configurações, etc.

## Subindo os serviços

Para subir todos os serviços, execute:
```bash
sudo docker-compose up
```

Flags opcionais:
* -d (detached): diz ao docker-compose para subir os containers de forma independente, sem console anexado
* --force-recreate: caso, por algum motivo, não perceba que o docker-compose não está recriando sua imagem, você pode tentar força a recriação da mesma

## Parando os serviços

Para parar todos os serviços, execute:
```bash
sudo docker-compose down
```

Flags opcionais:
* --help: obtém ajuda sobre o comando docker-compose
* --rmi local: diz ao docker-compose para remover as imagens dos serviços locais
