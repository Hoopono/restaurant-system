# 🚀 Setup GitHub Pages - Restaurant System

## ✅ PASSO 1: Configurações no Repositório

1. Acesse seu repositório: https://github.com/Hoopono/restaurant-system
2. Vá em **Settings** → **Pages**
3. Em "Source", selecione:
   - **Branch**: `gh-pages`
   - **Folder**: `/ (root)`
4. Clique em **Save**

---

## 🔧 PASSO 2: Configurar Localmente

### 2.1 Clone o repositório
```bash
git clone https://github.com/Hoopono/restaurant-system.git
cd restaurant-system
```

### 2.2 Instale as dependências
```bash
cd frontend
npm install
npm install --save-dev gh-pages
```

---

## 📦 PASSO 3: Build e Deploy

### 3.1 Primeira vez - Build
```bash
cd frontend
npm run build
```

### 3.2 Deploy para GitHub Pages
```bash
npm run deploy
```

✅ Seu site estará online em: **https://hoopono.github.io/restaurant-system/**

---

## 🔄 PASSO 4: Atualizar a Página (Futuro)

Sempre que fazer mudanças:

```bash
cd frontend
npm run deploy
```

Ou deixar automático (GitHub Actions já está configurado):
- Basta fazer `git push` no branch `main`
- GitHub Actions faz o deploy automaticamente! 🤖

---

## 🌐 URLs Disponíveis

- **Página Principal**: https://hoopono.github.io/restaurant-system/
- **Repositório**: https://github.com/Hoopono/restaurant-system

---

## 🧪 Dados de Teste

```
Email: teste@email.com
Senha: 123456
```

---

## ⚠️ OBSERVAÇÕES IMPORTANTES

1. **Primeira execução leva 2-5 minutos** ⏱️
2. **GitHub Pages precisa de 1-2 minutos para atualizar** 🔄
3. **O workflow automático (.github/workflows/deploy.yml) faz tudo** 🤖

---

## 🐛 Se não funcionar?

### Verificar GitHub Actions
1. Vá em **Actions** no seu repositório
2. Verifique se o workflow "Deploy" executou com sucesso ✅
3. Se falhou, clique nele para ver o erro

### Limpar Cache
```bash
rm -rf node_modules
npm install
npm run build
```

### Force Deploy
```bash
npm run deploy -- --nojekyll
```

---

## 📊 Status Atual

✅ Repositório criado  
✅ Código pronto  
✅ GitHub Actions configurado  
✅ Vite configurado para `/restaurant-system/`  
⏳ Aguardando primeiro deploy  

---

**Próximo passo:** Execute `npm run deploy` no seu terminal!
