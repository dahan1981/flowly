# Flowly

> Plataforma de automação de funis de vendas para micro-empreendedores brasileiros.

## 🚀 Deploy no GitHub Pages (passo a passo)

### 1. Criar repositório no GitHub

1. Acesse [github.com/new](https://github.com/new)
2. Dê o nome: `flowly` (ou qualquer nome que preferir)
3. Deixe **público**
4. Clique em **Create repository**

### 2. Subir os arquivos

Abra o terminal na pasta do projeto e rode:

```bash
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/flowly.git
git push -u origin main
```

> Substitua `SEU_USUARIO` pelo seu usuário do GitHub.

### 3. Ativar GitHub Pages

1. No repositório, vá em **Settings → Pages**
2. Em **Source**, selecione: **Deploy from a branch**
3. Em **Branch**, selecione: `main` / `/ (root)`
4. Clique em **Save**

Após 1-2 minutos, seu site estará disponível em:
```
https://SEU_USUARIO.github.io/flowly/
```

### 4. Domínio personalizado (opcional)

Se quiser usar seu próprio domínio (ex: `app.seudominio.com.br`):

1. Em **Settings → Pages → Custom domain**, coloque seu domínio
2. No painel do seu DNS, adicione um registro:
   - Tipo: `CNAME`
   - Nome: `app` (ou `www`)
   - Destino: `SEU_USUARIO.github.io`
3. Aguarde a propagação DNS (pode levar até 24h)

---

## 📁 Estrutura do projeto

```
flowly/
├── index.html   # App completo — tudo em um arquivo
├── logo.png     # Logo da Flowly
└── README.md    # Este arquivo
```

## ⚙️ Como funciona

Este projeto usa **React via CDN + Babel standalone** — não precisa de `npm install` nem `build`. Basta abrir o `index.html` no navegador ou subir direto no GitHub Pages.

## 🛠️ Próximos passos (quando escalar)

- [ ] Migrar para Vite + React (build otimizado)
- [ ] Adicionar React Router para URLs reais
- [ ] Conectar backend/API
- [ ] Autenticação de usuários
