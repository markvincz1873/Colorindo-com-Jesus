# Colorindo com Jesus - Deploy Package

Este pacote contém todos os arquivos necessários para fazer deploy da aplicação **Colorindo com Jesus** em qualquer plataforma de hospedagem.

## 📦 Conteúdo

- `dist/` - Aplicação compilada (frontend + backend)
  - `dist/public/` - Arquivos estáticos do frontend
  - `dist/index.js` - Servidor Express compilado
- `package.json` - Dependências de produção
- `README.md` - Este arquivo

## 🚀 Como fazer Deploy

### 1. Preparar o ambiente

Certifique-se de que sua plataforma de hospedagem suporta:
- **Node.js** versão 18 ou superior
- **NPM** ou **Yarn**

### 2. Fazer upload dos arquivos

Faça upload de todos os arquivos desta pasta para sua plataforma de hospedagem.

### 3. Instalar dependências

Execute no terminal da sua hospedagem:

```bash
npm install --production
```

### 4. Configurar porta

A aplicação está configurada para rodar na **porta 5000**.

Certifique-se de que sua plataforma esteja configurada para essa porta, ou ajuste a variável de ambiente `PORT` se necessário.

### 5. Iniciar a aplicação

Execute:

```bash
npm start
```

## 🌐 Plataformas Compatíveis

Esta aplicação pode ser hospedada em:

- **Vercel**
- **Heroku**
- **Railway**
- **Render**
- **DigitalOcean App Platform**
- **AWS (EC2, Elastic Beanstalk)**
- **Google Cloud Platform**
- Qualquer VPS com Node.js

## ⚙️ Variáveis de Ambiente (Opcional)

Se sua aplicação usar variáveis de ambiente, configure-as na sua plataforma:

- `PORT` - Porta do servidor (padrão: 5000)
- `NODE_ENV` - Ambiente de execução (use "production")

## 📝 Notas Importantes

1. A aplicação serve o frontend e backend na mesma porta
2. Os arquivos estáticos estão em `dist/public/`
3. O servidor Express está compilado em `dist/index.js`
4. Esta é uma aplicação fullstack - frontend React + backend Express

## 🆘 Suporte

Em caso de problemas no deploy, verifique:
- ✅ Node.js versão 18+ está instalado
- ✅ Todas as dependências foram instaladas corretamente
- ✅ A porta está configurada corretamente
- ✅ Os logs do servidor para identificar erros

## 📄 Estrutura da Aplicação

```
deploy-package/
├── dist/
│   ├── public/          # Frontend React buildado
│   │   ├── index.html
│   │   ├── assets/      # CSS, JS, imagens
│   └── index.js         # Servidor Express
├── package.json         # Dependências
└── README.md           # Este arquivo
```

---

**Desenvolvido com ❤️ para Colorindo com Jesus**
