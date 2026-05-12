# 🎨 GERADOR_TONY

Site exclusivo de geração de imagens com IA — acesso restrito apenas ao dono.

## 🔐 Credenciais de acesso

- **Usuário:** `tony`
- **Senha:** `tony123`

> ⚠️ Apenas o dono tem essa credencial. Para alterar, edite o arquivo `server.js` na seção `OWNER_CREDENTIALS`.

## 🚀 Como rodar

```bash
# 1. Instalar dependências
npm install

# 2. Iniciar o servidor
npm start

# 3. Abrir no navegador
http://localhost:3000
```

## ✨ Funcionalidades

- 🔒 Sistema de login com sessão (cookies httpOnly, 4h de validade)
- 🛡️ Todas as rotas do app e API protegidas — sem login não acessa nada
- 🎨 Geração real de imagens via **Pollinations.ai** (API gratuita, sem chave)
- 🤖 5 modelos de IA disponíveis: Flux, Flux Realism, Flux Anime, Flux 3D, Turbo
- 📐 Dimensões personalizáveis (256–1920 px)
- 🎯 Presets de prompts prontos
- 📚 Histórico da sessão
- ⬇️ Download direto das imagens
- 📱 Interface responsiva (mobile-friendly)

## 🛠️ Stack

- **Backend:** Node.js + Express + express-session
- **Frontend:** HTML/CSS/JS puro (sem framework)
- **IA:** Pollinations.ai (Flux models)

## 🔧 Como alterar a senha

Abra `server.js` e edite:

```javascript
const OWNER_CREDENTIALS = {
  username: 'tony',
  password: 'tony123'  // <-- troque aqui
};
```

## 📦 Deploy

Pode ser hospedado em:
- **Render.com** (grátis)
- **Railway.app**
- **Fly.io**
- **VPS próprio** (DigitalOcean, Hetzner, etc.)

Basta fazer `git push` e configurar a porta via variável `PORT`.
