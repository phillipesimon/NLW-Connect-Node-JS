🚀 NLW Connect (Backend)

Este é o backend do projeto NLW Connect, desenvolvido durante a NLW da Rocketseat. A API permite a inscrição de participantes em eventos, além de gerenciar convites e rankings.

🛠️ Tecnologias

Este projeto foi desenvolvido com as seguintes tecnologias:

Node.js - Ambiente de execução JavaScript no backend.

Fastify - Framework web rápido e eficiente para Node.js.

Drizzle ORM - ORM leve para TypeScript e SQL.

PostgreSQL - Banco de dados relacional utilizado no projeto.

Redis - Armazenamento em cache e sistema de mensagens.

Zod - Validação de esquemas de dados.

TypeScript - Superset do JavaScript com tipagem estática.

Swagger - Documentação automática da API.

📂 Estrutura do Projeto

📦 NLW-Connect-Node-JS  
┣ 📂 src  
┃ ┣ 📂 drizzle               # Configuração do banco de dados (Drizzle ORM)  
┃ ┃ ┣ 📜 client.ts  
┃ ┃ ┣ 📂 migrations          # Migrações do banco de dados  
┃ ┃ ┗ 📂 schema              # Definição dos esquemas das tabelas  
┃ ┣ 📂 functions             # Funções de negócio da aplicação  
┃ ┣ 📂 redis                 # Configuração do Redis  
┃ ┣ 📂 routes                # Rotas da API  
┃ ┣ 📜 env.ts                # Configuração de variáveis de ambiente  
┃ ┗ 📜 server.ts             # Arquivo principal do servidor  
┣ 📜 package.json            # Dependências e scripts do projeto  
┣ 📜 tsconfig.json           # Configuração do TypeScript  
┣ 📜 docker-compose.yml      # Configuração para rodar o projeto com Docker  
┗ 📜 drizzle.config.ts       # Configuração do Drizzle ORM  

🚀 Como rodar o projeto

1️⃣ Clone o repositório

git clone https://github.com/phillipesimon/NLW-Connect-Node-JS.git  

cd NLW-Connect-Node-JS  

2️⃣ Instale as dependências

npm install  

3️⃣ Configurar variáveis de ambiente

Crie um arquivo .env na raiz do projeto e defina as variáveis necessárias, como o banco de dados PostgreSQL e o Redis.

4️⃣ Rodar migrações do banco de dados

npm run drizzle:push  

5️⃣ Iniciar o servidor

npm run dev  

📖 API Endpoints

A documentação da API pode ser acessada via Swagger em:

http://localhost:3333/docs

🐳 Executando com Docker

Caso queira rodar o projeto com Docker, basta executar:

docker-compose up

Isso iniciará um container com PostgreSQL e Redis configurados.

📜 Licença

Este projeto está sob a licença MIT.
