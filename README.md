# 🥗 NutriGo – Plataforma Inteligente de Delivery Saudável

NutriGo é uma plataforma completa de delivery focada em alimentação saudável, conectando usuários a estabelecimentos parceiros com recomendações inteligentes, praticidade e segurança.

Mais que delivery, o NutriGo promove um estilo de vida saudável por meio da tecnologia.

---

# 📌 Visão Geral

A rotina moderna impacta diretamente os hábitos alimentares. O NutriGo surge como solução digital para:

- Facilitar o acesso a refeições saudáveis
- Oferecer recomendações personalizadas
- Conectar usuários a restaurantes comprometidos com bem-estar
- Garantir segurança e escalabilidade através de arquitetura moderna

---

# 🎯 Público-Alvo

- 👩‍💻 Jovens urbanos
- 👔 Profissionais com rotina intensa
- 🏋️ Público fitness
- 👨‍👩‍👧‍👦 Famílias conscientes

---

# 🚀 Funcionalidades

## 👤 Gestão de Usuários

- Cadastro de usuário
- Login autenticado com JWT
- Atualização de dados
- Histórico de pedidos
- Proteção de rotas

## 🛒 Sistema de Pedidos

- Criação de pedidos
- Listagem de pedidos
- Atualização de status
- Associação entre usuário e produtos

## 🏪 Parceiros e Produtos

- Cadastro de estabelecimentos
- Listagem de restaurantes
- Produtos vinculados a parceiros
- Sistema de busca e filtragem

---

# 🧠 Arquitetura do Sistema

## Frontend

- React
- TypeScript
- Vite
- Axios
- Context API

Repositório:
https://github.com/Grupo-02-Turma-JavaScript-12/NutriGo-Delivery-Frontend

Estrutura principal:

A comunicação ocorre via HTTP utilizando Axios, garantindo separação clara entre camada de apresentação e camada de negócio.

A aplicação frontend foi construída com:

- React
- TypeScript
- Vite
- Axios
- Context API

Repositório:
https://github.com/Grupo-02-Turma-JavaScript-12/NutriGo-Delivery-Frontend

A API foi desenvolvida com:

- NestJS
- TypeORM
- PostgreSQL
- JWT
- Passport
- Bcrypt
- Swagger
- Supertest

A organização segue padrão modular por domínio, contendo controllers, services, entities, DTOs e guards, garantindo escalabilidade e manutenção simplificada.

---

# 🗄️ Modelo de Dados

O banco de dados relacional utiliza PostgreSQL, com mapeamento via TypeORM.

Principais entidades:

- User
- Pedido
- Parceiro
- Produto

Relacionamentos implementados:

- Um usuário pode possuir múltiplos pedidos
- Um parceiro pode possuir múltiplos produtos
- Um pedido pode conter múltiplos produtos

Essa modelagem garante integridade referencial e organização da regra de negócio.

---

# 🔐 Segurança

A autenticação é baseada em JWT (JSON Web Token).

Fluxo implementado:

1. Usuário envia credenciais para POST /auth/login
2. A senha é validada utilizando bcrypt
3. Um token JWT é gerado
4. O token deve ser enviado no header:
   Authorization: Bearer {token}
5. Guards validam automaticamente o token em rotas protegidas

O sistema também implementa:

- Validação de dados via DTOs
- Bloqueio de usuários duplicados
- Estrutura de camadas para evitar exposição indevida de dados

---

# 📚 Documentação da API

A documentação interativa da API está disponível via Swagger:

https://nutrigo-delivery.onrender.com/swagger

Através do Swagger é possível:

- Visualizar todos os endpoints
- Testar requisições
- Ver modelos de dados
- Conferir exemplos de payload
- Validar autenticação

Principais endpoints disponíveis:

- POST /auth/login
- POST /users
- GET /users
- PUT /users/:id
- POST /pedidos
- GET /pedidos
- GET /parceiros
- POST /parceiros
- GET /produtos

---

# 🧪 Testes

O backend possui testes automatizados E2E utilizando:

- NestJS Testing Module
- Supertest
- SQLite em ambiente isolado

Os testes cobrem:

- Cadastro de usuários
- Bloqueio de duplicidade
- Login com geração de token
- Acesso a rotas protegidas
- Validação de autenticação

---

# ⚙️ Como Executar o Projeto

Backend:

npm install  
npm run start:dev

Swagger local:
http://localhost:3000/swagger

Frontend:

git clone https://github.com/Grupo-02-Turma-JavaScript-12/NutriGo-Delivery-Frontend  
cd NutriGo-Delivery-Frontend  
npm install  
npm run dev

Frontend disponível em:
http://localhost:5173

---

# ☁️ Deploy

O backend está hospedado na plataforma Render, com documentação pública ativa em ambiente de produção.

https://nutrigo-delivery.onrender.com/swagger

---

# 🌱 Diferenciais Técnicos

- Arquitetura Fullstack desacoplada
- API REST documentada com Swagger
- Segurança robusta com JWT e bcrypt
- Estrutura modular escalável
- Testes automatizados E2E
- Interface moderna com React + Vite
- Separação clara de responsabilidades entre camadas

---

# 💚 Missão

Promover saúde, praticidade e tecnologia em cada refeição, tornando a alimentação saudável mais acessível e conveniente.

NutriGo – Saúde que chega até você.

---

# 👨‍💻 Equipe

Projeto desenvolvido pelo Grupo 02 – Turma JavaScript 12.
