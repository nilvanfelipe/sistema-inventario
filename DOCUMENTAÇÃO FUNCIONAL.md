# 📘 DOCUMENTAÇÃO FUNCIONAL

# Sistema de Inventário com Governança e Inventário Cíclico

---

# 1️⃣ Visão Geral do Produto

## 🎯 Objetivo

Desenvolver um aplicativo de controle de inventário com:

- Governança
- Inventário cíclico
- Controle de divergência
- Auditoria completa
- Preparação para BI
- Estrutura preparada para SaaS (multiempresa)

---

# 2️⃣ Escopo do Produto

O sistema será composto por 8 módulos principais:

1. Gestão de Usuários
2. Gestão de Empresas (multi-tenant)
3. Cadastro de Produtos
4. Gestão de Localizações
5. Movimentações de Estoque
6. Inventário Cíclico
7. Governança e Auditoria
8. Relatórios e Indicadores

---

# 3️⃣ Módulos e Funcionalidades

## 🔐 3.1 Gestão de Usuários

- Cadastro, login JWT, reset de senha
- Perfis: Administrador, Operador, Auditor, Gestor
- Cada usuário pertence a uma empresa

## 🏢 3.2 Gestão de Empresas (Multiempresa)

- Cadastro, ativação/desativação
- Configurações: saldo negativo, tolerância, frequência de inventário

## 📦 3.3 Cadastro de Produtos

- CRUD com soft delete, classificação ABC
- SKU, código de barras, unidade de medida, categoria

## 📍 3.4 Gestão de Localizações

- Estrutura hierárquica: Armazém → Rua → Prateleira → Posição

## 🔄 3.5 Movimentações de Estoque

- Tipos: Entrada, Saída, Transferência, Ajuste
- Saldo = soma das movimentações (ledger)

## 📊 3.6 Inventário Cíclico

- Cronograma por classe ABC, ordens de contagem
- Workflow de aprovação, segunda contagem

## 🧾 3.7 Governança e Auditoria

- Log completo de ações, histórico de ajustes

## 📈 3.8 Indicadores e Relatórios

- Acuracidade, taxa de divergência, exportação CSV/Excel

---

# 6️⃣ Fluxos Críticos

- **Entrada**: Compra → Registro → Saldo atualizado
- **Inventário**: Lista → Contagem → Divergência → Aprovação → Ajuste
- **Ajuste**: Solicitação → Justificativa → Aprovação → Registro
