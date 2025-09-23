# 🌐 Webdojo – Testes Automatizados com Cypress

Este repositório contém a aplicação **Webdojo** e uma suíte de **testes automatizados** desenvolvida em [Cypress](https://www.cypress.io/).  
O objetivo é validar as principais funcionalidades da aplicação e garantir sua qualidade de forma contínua.

---

## 📁 Estrutura do Projeto

A pasta `cypress` contém toda a automação de testes, organizada da seguinte forma:

```
cypress/
├─ e2e/               # Arquivos de testes end-to-end (.cy.js)
├─ fixtures/          # Massa de dados e arquivos para os testes
│  ├─ cep.json
│  ├─ consultancy.json
│  └─ document.pdf
├─ support/           # Comandos e funções de suporte
│  ├─ actions/        # Ações reutilizáveis em testes
│  │  └─ consultancy.actions.js
│  ├─ commands.js     # Comandos customizados do Cypress
│  ├─ e2e.js          # Configurações globais para testes e2e
│  └─ utils.js        # Funções utilitárias
```

---

## 🚀 Configuração do Ambiente

### 1️⃣ Clonar o repositório
```bash
git clone <URL_DO_REPOSITORIO>
cd <PASTA_DO_PROJETO>
```

### 2️⃣ Instalar as dependências
```bash
npm install
```

### 3️⃣ Rodar a aplicação Webdojo
A aplicação está no mesmo repositório. Para iniciá-la:
```bash
npm run dev
```
Acesse em: [http://localhost:3000](http://localhost:3000)

---

## 🧪 Executando os Testes

Os testes podem ser executados em **modo headless** (linha de comando) ou pela **interface gráfica** do Cypress.

### Scripts disponíveis

| Comando                   | Descrição                                                                 |
|-----------------------------|---------------------------------------------------------------------------|
| `npm run test`              | Executa todos os testes em modo headless com viewport **1440x900**        |
| `npm run test:ui`           | Abre a interface interativa do Cypress                                   |
| `npm run test:login`        | Executa apenas o teste `login.cy.js` em modo headless (viewport **1440x900**) |
| `npm run test:login:mobile` | Executa `login.cy.js` simulando viewport **414x896** (modo mobile)        |

Exemplo:
```bash
npm run test
```

> ⚠️ **Importante:** Certifique-se de que a aplicação **Webdojo** esteja rodando (`npm run dev`) antes de iniciar os testes.

---

## 💡 Dicas Úteis

- Arquivos em `cypress/fixtures` armazenam **massa de dados** e podem ser alterados conforme a necessidade.
- **Comandos customizados** podem ser adicionados em `cypress/support/commands.js` para reaproveitar ações comuns.
- Use a interface (`npm run test:ui`) para depuração mais visual e desenvolvimento de novos testes.

---

## 🛠️ Tecnologias

- [Node.js](https://nodejs.org/)
- [Cypress](https://www.cypress.io/)

---


