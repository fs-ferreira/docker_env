[![Continuous Deploy with Github](https://github.com/fs-ferreira/docker_env/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/fs-ferreira/docker_env/actions/workflows/docker-publish.yml)

# Ambiente de microserviços em containers docker

Projeto desenvolvido para demonstrar as principais ferramentas de desenvolvimento de microserviços, visando as melhores práticas e com as bibliotecas mais atuais.

Todo o projeto foi feito com Spring 3.2.3 e Java 21;

O que contêm nesse projeto:
- Microserviços de Câmbio e Livro
    - Desenvolvidos com padrão REST
    - OpenApi docs
    - Feign Client
    - Reslience4j
- Eureka Naming Server - Responsável por fazer o load balance dos demais microserviços permitindo sua escabilidade e performance.
- API Gateway - Centralizador de rotas dos microserviços
- Zipkin/Micrometer - Rastreamento de rotas entre microserviços
    - Intergado ao rabbitMQ
- Integração contínua e automática por push detection
    - Github Actions
    - Docker Hub
- Submódulos do Github


## Como rodar localmente a aplicação

1. Clone o repositório com --recursive para clonar os submódulos

    ```bash
    git clone --recursive https://github.com/fs-ferreira/docker_env.git
    ````
2. Acesse o projeto

    ```bash
    cd docker_env
    ````
3. Execute o docker compose

    ```bash
    docker compose up -d
    ````


## Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir sugerir melhorias e apontar possíveis issues no projeto.

