# 🚀 Root Portfolio

![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-5-646CFF?logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-3-38B2AC?logo=tailwindcss&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
![Fork](https://img.shields.io/badge/Fork-adaptado-orange)

> 🍴 **Este repositório é um FORK de [`codedbyflow/Root-Portfolio`](https://github.com/codedbyflow/Root-Portfolio)**, projeto original de **Kaio Silva** ([@codedbyflow](https://github.com/codedbyflow)), sob licença **MIT**.
> Adaptado e mantido por **[Isaque Félix](https://github.com/isaquefl)** com melhorias de segurança, documentação e organização. Todo o crédito do código original permanece com o autor.

Portfólio digital interativo e animado, desenvolvido com **React 18**, **Vite** e **Tailwind CSS**, com seções de projetos, skills, depoimentos e formulário de contato integrado ao Discord via webhook.

## ✨ Funcionalidades

- Página inicial animada com Framer Motion
- Showcase interativo de projetos com filtros e modal de detalhes
- Matriz de habilidades (skills) e grade de tech stack
- Seção de depoimentos e estatísticas
- Formulário de contato que envia mensagens direto para um canal do Discord (webhook)
- Deploy pronto para Vercel (`vercel.json` incluso)

## 🛠️ Tecnologias

- React 18 + React Router 6
- Vite 5
- Tailwind CSS 3 (forms, typography, container queries, fluid type)
- Framer Motion
- Redux Toolkit
- Recharts / D3

## 🚀 Como executar

```bash
# 1. Clone o repositório
git clone https://github.com/isaquefl/Root-Portfolio.git
cd Root-Portfolio

# 2. Instale as dependências
npm install

# 3. Configure as variáveis de ambiente
cp .env.example .env
# edite o .env com seus valores

# 4. Inicie em modo de desenvolvimento
npm start

# Build de produção
npm run build
```

## ⚙️ Configuração (.env)

| Variável | Obrigatória | Descrição |
| --- | --- | --- |
| `VITE_DISCORD_WEBHOOK_URL` | Para o formulário de contato | URL do webhook do Discord que recebe as mensagens do site |

Sem a variável configurada, o site funciona normalmente — apenas o envio do formulário de contato fica desativado (com aviso no console).

> ⚠️ **Nunca** faça commit do arquivo `.env`. Use sempre o `.env.example` como modelo.

## 🔒 Melhorias aplicadas neste fork

- **Segurança**: removida URL de webhook do Discord que estava _hardcoded_ no código (`ContactSection.jsx`) — agora é lida de `import.meta.env.VITE_DISCORD_WEBHOOK_URL`, com fallback seguro quando ausente
- **`.env.example`** padronizado e bilíngue
- **`.gitignore`** reforçado (`.env`, `dist/`, `node_modules`, logs)
- **README** profissional e bilíngue (PT/EN), com créditos ao autor original

## 📞 Contato

- **Autor original**: Kaio Silva — [@codedbyflow](https://github.com/codedbyflow) · [@roootunk](https://github.com/roootunk) · [rootunk.xyz](https://rootunk.xyz)
- **Fork mantido por**: [Isaque Félix](https://github.com/isaquefl)

## 📄 Licença

Distribuído sob a licença **MIT**. Veja o arquivo [`LICENSE`](LICENSE) para detalhes.
Copyright (c) Kaio Silva.

---

# 🚀 Root Portfolio (English)

> 🍴 **This repository is a FORK of [`codedbyflow/Root-Portfolio`](https://github.com/codedbyflow/Root-Portfolio)**, originally created by **Kaio Silva** ([@codedbyflow](https://github.com/codedbyflow)) under the **MIT** license.
> Adapted and maintained by **[Isaque Félix](https://github.com/isaquefl)** with security, documentation and organization improvements. Full credit for the original code remains with the author.

An interactive, animated developer portfolio built with **React 18**, **Vite** and **Tailwind CSS**, featuring a project showcase, skills matrix, testimonials and a contact form integrated with Discord via webhook.

## ✨ Features

- Animated landing page (Framer Motion)
- Interactive project showcase with filters and detail modal
- Skills matrix and tech stack grid
- Testimonials and stats sections
- Contact form that posts messages to a Discord channel (webhook)
- Vercel-ready deployment (`vercel.json` included)

## 🚀 Getting Started

```bash
git clone https://github.com/isaquefl/Root-Portfolio.git
cd Root-Portfolio
npm install
cp .env.example .env   # then fill in your values
npm start              # dev server
npm run build          # production build
```

## ⚙️ Configuration (.env)

| Variable | Required | Description |
| --- | --- | --- |
| `VITE_DISCORD_WEBHOOK_URL` | For the contact form | Discord webhook URL that receives site messages |

Without it, the site still works — only the contact form submission is disabled (console warning).

## 🔒 Improvements in this fork

- **Security**: removed a hardcoded Discord webhook URL from `ContactSection.jsx` — now read from `import.meta.env.VITE_DISCORD_WEBHOOK_URL` with a safe fallback
- Standardized bilingual **`.env.example`**
- Hardened **`.gitignore`** (`.env`, `dist/`, `node_modules`, logs)
- Professional bilingual **README** with proper credits

## 📄 License

Licensed under the **MIT** License — see [`LICENSE`](LICENSE). Copyright (c) Kaio Silva.

---

*Desenvolvido com ❤️ por Kaio Silva — fork mantido por Isaque Félix.*
