# 🥗 NutriGo – Plataforma Inteligente de Delivery Saudável

NutriGo é uma plataforma digital de delivery focada em alimentação saudável, desenvolvida para conectar usuários a restaurantes parceiros por meio de uma experiência moderna, segura e escalável.

A aplicação foi construída com foco em **arquitetura organizada, boas práticas de frontend moderno e integração segura com API REST**, promovendo não apenas pedidos online, mas um ecossistema voltado ao bem-estar.

---

## 📌 Visão do Produto

A rotina contemporânea impacta diretamente os hábitos alimentares. O NutriGo surge como uma solução tecnológica para:

- Facilitar o acesso a refeições saudáveis
- Oferecer uma navegação intuitiva e rápida
- Garantir autenticação segura com JWT
- Integrar usuários e estabelecimentos em um sistema escalável

O projeto foi estruturado pensando em **experiência do usuário, manutenibilidade e crescimento futuro da aplicação**.

---

## 🎯 Público-Alvo

- 👩‍💻 Jovens urbanos
- 👔 Profissionais com rotina intensa
- 🏋️ Público fitness
- 👨‍👩‍👧‍👦 Famílias que buscam alimentação equilibrada

---

## 🚀 Funcionalidades Implementadas

### 👤 Gestão de Usuários

- Cadastro e autenticação com token JWT
- Persistência de sessão
- Proteção de rotas privadas
- Atualização de dados cadastrais
- Histórico de pedidos

### 🛒 Sistema de Pedidos

- Criação de pedidos
- Listagem por usuário autenticado
- Atualização de status
- Relacionamento entre usuários, produtos e estabelecimentos

### 🏪 Restaurantes e Produtos

- Cadastro e listagem de parceiros
- Produtos vinculados aos restaurantes
- Sistema de busca e filtragem
- Renderização dinâmica baseada na API

---

## 🧠 Arquitetura do Frontend

A aplicação segue o padrão **SPA (Single Page Application)** com separação clara de responsabilidades.

### 🔹 Estrutura Modular

```bash
src/
 ├── assets/        # Arquivos estáticos
 ├── components/    # Componentes reutilizáveis
 ├── pages/         # Páginas da aplicação
 ├── services/      # Configuração do Axios e consumo da API
 ├── contexts/      # Gerenciamento global (AuthContext)
 ├── models/        # Interfaces e tipagens TypeScript
 ├── routes/        # Rotas públicas e privadas
 ├── App.tsx
 └── main.tsx
```

### 🔹 Padrões Utilizados

- Componentização e reutilização de código
- Context API para controle global de autenticação
- Interceptors do Axios para injeção automática do token JWT
- Separação entre camada de visualização e camada de serviços
- Tipagem forte com TypeScript

---

## 🛠️ Stack Tecnológica

- **React** — Construção da interface
- **TypeScript** — Segurança e escalabilidade
- **Vite** — Build rápido e ambiente otimizado
- **Axios** — Comunicação com API REST
- **React Router DOM** — Gerenciamento de rotas
- **Context API** — Estado global de autenticação

---

## 🔐 Fluxo de Autenticação

1. Usuário realiza login.
2. Backend retorna um token JWT.
3. Token é armazenado no `localStorage`.
4. Axios adiciona automaticamente o header `Authorization` nas requisições protegidas.
5. Rotas privadas validam autenticação antes de renderizar páginas sensíveis.

---

## ⚙️ Configuração do Ambiente

Crie um arquivo `.env` na raiz do projeto:

```bash
VITE_API_URL=http://localhost:8080
```

---

## 🧪 Como Executar o Projeto

Clone o repositório:

```bash
git clone https://github.com/Grupo-02-Turma-JavaScript-12/NutriGo-Delivery-Frontend
cd NutriGo-Delivery-Frontend
```

Instale as dependências:

```bash
npm install
```

Execute o projeto:

```bash
npm run dev
```

Acesse no navegador:

```
http://localhost:5173
```

---

## 📈 Evoluções Futuras

- Implementação de carrinho persistente
- Sistema de avaliação de restaurantes
- Integração com gateway de pagamento
- Testes automatizados (Jest / React Testing Library)
- Pipeline CI/CD
- Deploy em ambiente cloud (Vercel ou similar)

---

## 👨‍💻 Desenvolvimento

Projeto desenvolvido em equipe com foco em práticas modernas de desenvolvimento frontend, organização arquitetural e integração com backend REST.
