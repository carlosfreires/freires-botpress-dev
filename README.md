# freires-botpress-dev

Este repositório contém uma configuração pronta para você iniciar rapidamente com o Botpress utilizando Docker.  
O objetivo é facilitar a criação e personalização de chatbots, utilizando a versão mais recente do Botpress disponível em 27 janeiro de 2025.

## Índice

- [Sobre o Projeto](#sobre-o-projeto)
- [Tecnologias Usadas](#tecnologias-usadas)
- [Como Rodar Localmente](#como-rodar-localmente)
  - [Requisitos](#requisitos)
  - [Passo a Passo](#passo-a-passo)
  - [Iniciar o Container](#iniciar-o-container)
  - [Parar o Container](#parar-o-container)
  - [Acessar o Botpress no Container](#acessar-o-botpress-no-container)
- [Branch `chatbots`](#branch-chatbots)
- [Referências](#referências)

## Sobre o Projeto

O **Botpress** é uma plataforma poderosa para criar chatbots de forma simples e sem a necessidade de grandes esforços de codificação. Este repositório contém um contêiner Docker configurado com o Botpress para facilitar a criação de chatbots em seu ambiente local.

### Docker

O projeto utiliza **Docker** para empacotar e isolar a aplicação do Botpress em um ambiente controlado. Com o uso de containers, você pode facilmente rodar e desenvolver chatbots localmente, sem se preocupar com dependências ou configurações complicadas.

## Tecnologias Usadas

- **Botpress**: Plataforma para construção de chatbots.
- **Docker**: Plataforma para automação de implantação de aplicativos em containers.

## Como Rodar Localmente

### Requisitos

- **Docker**: O Docker deve estar instalado em sua máquina. Você pode [baixá-lo aqui](https://www.docker.com/get-started).
- **Git**: Para clonar o repositório.

### Passo a Passo

1. **Clone este repositório** para sua máquina:

    ```bash
    git clone https://github.com/SEU_USUARIO/freires-botpress-dev.git
    ```

2. **Navegue até o diretório do repositório clonado**:

    ```bash
    cd freires-botpress-dev
    ```

3. **Construa e inicie o container Docker** com o comando:

    ```bash
    docker-compose up -d
    ```

    Isso irá:
    - Baixar a imagem do Docker `freires/botpress-server:latest-version-as-of-01.26.2025` (a versão mais recente disponível do Botpress na data de 27/01/2025).
    - Mapear a porta `3000` para acessar o painel do Botpress no seu navegador.
    - Criar volumes para persistir os dados do Botpress e para mapear o repositório local para o container, caso necessário.

4. **Acesse o Botpress no seu navegador**:
   
   Abra o navegador e acesse `http://localhost:3000`. Você verá a interface de administração do Botpress, onde pode começar a criar e gerenciar seus chatbots.

#### ▶️ **Iniciar o Container**

Para iniciar o container, use o seguinte comando:
```bash
docker-compose up -d
```

#### ⏹️ **Parar o Container**

Para parar o container, utilize:
```bash
docker-compose down
```

#### ⚙️ **Acessar o Botpress no Container**

Para acessar o Botpress diretamente no terminal dentro do container, use o comando:
```bash
docker exec -it freires-botpress-dev_botpress_1 bash
```

Após isso, você estará dentro do container, onde poderá realizar algumas configurações avançadas ou verificar os logs.

## Branch chatbots
Estou trabalhando na branch chatbots, onde você encontrará alguns chatbots prontos, criados por mim. Fique à vontade para usar, testar e otimizar os bots de acordo com suas necessidades!

Para acessar a branch, utilize o seguinte comando:
```bash
git checkout chatbots
```

### Referências

Para mais informações sobre como criar, configurar e personalizar seus chatbots, consulte a documentação oficial do Botpress.

Para aprender mais sobre o Docker e como ele funciona, consulte a documentação oficial do Docker.

Divirta-se criando seus chatbots! 🚀