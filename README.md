
# Projeto Minsait - Cadastramento de Operações

Este projeto é uma aplicação web que permite que gestores e usuários cadastrem novas operações em um fluxo dividido em etapas. O sistema garante que todas as informações sejam inseridas de forma organizada e com persistência em banco de dados relacional. A aplicação está contêinerizada com Docker Compose, utilizando o Quarkus (Java) para o backend, Angular para o frontend e PostgreSQL ou MySQL como banco de dados.

## Tecnologias Utilizadas

- **Frontend**: Angular (com TypeScript)
- **Backend**: Quarkus (Java)
- **Banco de Dados**: PostgreSQL ou MySQL
- **Docker**: Para contêinerização e orquestração com Docker Compose
- **Git**: Controle de versão e integração com repositório remoto

## Estrutura do Projeto

- **cadastramento-operacoes**: Diretório que contém o backend desenvolvido com Quarkus.
- **docker-compose.yml**: Arquivo de configuração do Docker Compose, que define os containers para o backend e o banco de dados.
- **src**: Diretório do frontend desenvolvido com Angular.
- **node_modules**: Dependências do Node.js para o frontend.
- **dist**: Diretório de saída após a compilação do frontend.

## Funcionalidades

- Cadastro de novas operações.
- Fluxo de etapas para cadastrar informações.
- Persistência de dados no banco de dados relacional.
- Interface de usuário interativa com o Angular.
- Backend robusto e seguro com Quarkus.
- Contêinerização para fácil implantação usando Docker Compose.

## Como Executar o Projeto

### Pré-requisitos

- [Docker](https://www.docker.com/get-started) instalado no seu sistema.
- [Node.js](https://nodejs.org/) instalado para rodar o Angular (somente para o frontend).
- [Git](https://git-scm.com/) para controle de versão.

### Passos para Rodar o Projeto

1. **Clone o repositório**:

   Clone o repositório para sua máquina local:

   ```bash
   git clone https://github.com/Arthurflsimao/projeto-minsait.git
   cd projeto-minsait
   ```

2. **Suba os containers com Docker Compose**:

   Com o Docker e o Docker Compose instalados, execute o comando abaixo para rodar o backend e o banco de dados:

   ```bash
   docker-compose up
   ```

   Isso irá criar os containers necessários para o backend e o banco de dados.

3. **Rodar o Frontend**:

   No diretório `src` do frontend, instale as dependências do Node.js e inicie o servidor de desenvolvimento:

   ```bash
   cd src
   npm install
   npm start
   ```

   Isso irá abrir o frontend no seu navegador, geralmente na URL `http://localhost:4200`.

4. **Acessando a Aplicação**:

   O frontend estará disponível em `http://localhost:4200`, enquanto o backend estará rodando nos containers Docker.

### Configurações

- **Banco de Dados**: O banco de dados está configurado no arquivo `docker-compose.yml`, onde você pode escolher entre PostgreSQL ou MySQL. Certifique-se de configurar corretamente os parâmetros de conexão do banco de dados conforme necessário.
  
- **Variáveis de Ambiente**: As configurações do backend (como conexão com o banco de dados) podem ser alteradas nas variáveis de ambiente ou no arquivo `application.properties` do Quarkus.

## Licença

Este projeto está sob a licença MIT. Consulte o arquivo [LICENSE](LICENSE) para mais detalhes.

## Contato

- **Autor**: Arthur Felix Latorre Simão
- **Email**: afelixl@minsait.com
