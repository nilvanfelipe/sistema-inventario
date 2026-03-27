# Sistema de Inventário com Governança e Inventário Cíclico

Sistema de controle de inventário multiempresa com inventário cíclico, governança e auditoria completa.

## 🚀 Stack Tecnológica

- **Backend**: Node.js + Express + TypeScript + Prisma
- **Frontend**: React + Vite + TypeScript
- **Banco de Dados**: PostgreSQL (ou SQLite para dev)
- **Autenticação**: JWT + bcrypt

## 📁 Estrutura do Projeto

```
projeto-apps-inventário/
├── backend/          # API REST
├── frontend/         # Interface React
├── database/         # Migrations e seeds
└── docs/             # Documentação
```

## ⚡ Como Executar

### Backend
```bash
cd backend
npm install
cp .env.example .env  # Configure as variáveis
npx prisma migrate dev
npm run dev
```

### Frontend
```bash
cd frontend
npm install
npm run dev
```

### Banco de Dados
Crie um arquivo `backend/.env` com:
```
DATABASE_URL="postgresql://user:password@localhost:5432/inventario"
JWT_SECRET="sua-chave-secreta"
```

## 📋 Módulos

1. 🔐 Gestão de Usuários
2. 🏢 Gestão de Empresas (multi-tenant)
3. 📦 Cadastro de Produtos
4. 📍 Gestão de Localizações
5. 🔄 Movimentações de Estoque
6. 📊 Inventário Cíclico
7. 🧾 Governança e Auditoria
8. 📈 Relatórios e Indicadores

## 📚 Documentação

- [Documentação Funcional](./DOCUMENTAÇÃO%20FUNCIONAL.md)
- [06 - Integração e APIs](./docs/06%20-%20Integração%20e%20APIs.md)
- [11 - Testes e Qualidade](./docs/11%20-%20Testes%20e%20Qualidade.md)
- [12 - Roadmap](./docs/12%20-%20Roadmap.md)
