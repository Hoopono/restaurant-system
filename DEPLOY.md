# 🚀 GUIA DE DEPLOY - Restaurant System

## ⚡ DEPLOY RÁPIDO (5 MINUTOS)

### Opção 1: Vercel (Recomendado) ✨

1. Acesse: https://vercel.com/new
2. Clique em "Import Git Repository"
3. Selecione: `Hoopono/restaurant-system`
4. Configure:
   - **Framework Preset**: Other
   - **Root Directory**: `./`
5. Clique em "Deploy"

✅ Seu site estará online em: `https://restaurant-system-<seu-nome>.vercel.app`

---

### Opção 2: GitHub Pages + Vercel

1. Fork o repositório
2. Ative GitHub Pages nas settings
3. Deploy automático a cada push

---

## 💻 EXECUTAR LOCALMENTE

### Requisitos
- Node.js 16+ instalado
- Git instalado

### Passo 1: Clonar
```bash
git clone https://github.com/Hoopono/restaurant-system.git
cd restaurant-system
```

### Passo 2: Backend (Terminal 1)
```bash
cd backend
npm install
npm start
```

Resultado:
```
🍽️ Servidor rodando em http://localhost:5000
```

### Passo 3: Frontend (Terminal 2)
```bash
cd frontend
npm install
npm run dev
```

Resultado:
```
➜ Local: http://localhost:5173/
```

### Passo 4: Abrir no navegador
- URL: http://localhost:5173

---

## 📱 DADOS DE TESTE

```
Email: teste@email.com
Senha: 123456
```

---

## 🌐 URLs DISPONÍVEIS

| Página | URL |
|--------|-----|
| Login | / |
| Dashboard | /dashboard |
| Cardápio | /cardapio |
| Comanda | /comanda |

---

## 🔧 VARIÁVEIS DE AMBIENTE

Criar arquivo `backend/.env`:

```env
PORT=5000
NODE_ENV=development
MONGODB_URI=mongodb://localhost:27017/restaurant-system
JWT_SECRET=sua-chave-super-segura
JWT_EXPIRE=7d
MERCADO_PAGO_TOKEN=seu-token
FRONTEND_URL=http://localhost:5173
```

---

## 📊 ESTRUTURA DO PROJETO

```
restaurant-system/
├── frontend/                 # React + Vite
│   ├── src/
│   │   ├── pages/           # Login, Dashboard, Cardápio, Comanda
│   │   ├── App.jsx          # Roteamento
│   │   └── index.css        # Tailwind
│   ├── index.html
│   └── package.json
├── backend/                  # Node.js + Express
│   ├── src/
│   │   └── server.js        # API
│   └── package.json
├── vercel.json              # Config deploy
└── README.md
```

---

## 🎯 PRÓXIMOS PASSOS

1. ✅ Integração com MongoDB
2. ✅ Autenticação JWT completa
3. ✅ Integração Mercado Pago
4. ✅ CRUD completo
5. ✅ Relatórios
6. ✅ Versão Desktop (Electron)

---

**Status**: ✅ Pronto para Deploy
**Versão**: 1.0.0
**Tecnologia**: React 18 + Node.js + Tailwind CSS
