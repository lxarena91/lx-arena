# ⚽ LX Arena App

LX Arena é uma aplicação moderna e responsiva construída com Next.js, Tailwind CSS e Supabase. O objetivo é conectar jogadores de futebol, futsal e futebol 7 em Lisboa, permitindo-lhes participar de jogos, reservar campos, ver estatísticas e criar partidas privadas com amigos.

---

## 🚀 Funcionalidades

- Autenticação (email/senha + Google)
- Listagem de jogos públicos
- Reservas com vagas controladas
- Painel de perfil com histórico
- Painel de admin com estatísticas e gestão de jogos
- Upload de imagem para jogos (via Supabase Storage)
- Filtros por local e hora

---

## 🧰 Tecnologias

- **Next.js (App Router + TypeScript)**
- **Tailwind CSS**
- **Supabase** (Auth, Database, Storage)
- **Stripe** (para futura integração de pagamentos)
- **Recharts** (gráficos interativos no painel admin)

---

## 📦 Instalação local

```bash
git clone https://github.com/lxarena91/lx-arena.git
cd lx-arena
npm install
```

Cria um arquivo `.env.local` na raiz com as tuas chaves:

```env
NEXT_PUBLIC_SUPABASE_URL=https://<teu-projeto>.supabase.co
NEXT_PUBLIC_SUPABASE_ANON_KEY=<tua-chave-anon>
```

Depois inicia o servidor:

```bash
npm run dev
```

A app estará em `http://localhost:3000`

---

## 🗂️ Estrutura de Pastas

```
/src
├─ app             → Rotas principais (/jogos, /perfil, /admin, etc)
├─ components      → Componentes reutilizáveis (Navbar, Cards)
├─ lib             → Supabase client
├─ styles          → Estilos globais se necessário
```

---

## 🌐 Deploy

Para fazer deploy da app em produção:

1. Usa [Vercel](https://vercel.com) e liga ao repositório GitHub
2. Adiciona as variáveis de ambiente do Supabase
3. Faz deploy 🚀

---

## 📄 Arquivos recomendados

### .gitignore
```gitignore
# dependencies
/node_modules

# production
/.next
/out

# misc
.DS_Store
.env
.env.local
.env.*.local

# logs
npm-debug.log*
yarn-debug.log*
yarn-error.log*

# Supabase
/supabase/.temp
/supabase/migrations/.supabase

# OS
Thumbs.db
```

### LICENSE (MIT)
```
MIT License

Copyright (c) 2025 Kelson

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 📩 Contato

Caso queiras colaborar ou tirar dúvidas:
- 📧 lxarena.app@gmail.com
- 🌍 [Em breve: https://lxarena.com](https://lxarena.com)

---

**LX Arena – O jogo começa contigo.**

