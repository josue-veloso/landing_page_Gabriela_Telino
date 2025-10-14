# Guia de Hospedagem - Landing Page Gabriela Telino

## 📋 Arquivos Necessários

Certifique-se de ter todos os arquivos:
- `index.html`
- `style.css`
- `script.js`
- Pasta `images/` com as fotos (banner.jpg e site.jpg)

---

## 🚀 Opções de Hospedagem GRATUITAS

### 1. **Netlify** (Recomendado - Mais Fácil)

**Vantagens:**
- 100% gratuito
- HTTPS automático
- Domínio personalizado gratuito
- Deploy em segundos

**Passo a passo:**

1. Acesse [netlify.com](https://www.netlify.com)
2. Clique em "Sign up" (pode usar conta do GitHub, Google ou email)
3. Após login, clique em "Add new site" → "Deploy manually"
4. Arraste a pasta `landing_page_Gabi` inteira para a área indicada
5. Aguarde o upload e deploy (30 segundos)
6. Pronto! Seu site estará no ar com um link tipo: `nome-aleatorio.netlify.app`

**Para usar domínio próprio:**
- Vá em "Domain settings"
- Clique em "Add custom domain"
- Siga as instruções para configurar seu domínio

---

### 2. **Vercel**

**Vantagens:**
- Gratuito
- Muito rápido
- HTTPS automático
- Ótima performance

**Passo a passo:**

1. Acesse [vercel.com](https://vercel.com)
2. Clique em "Sign Up" (pode usar GitHub, GitLab ou email)
3. Após login, clique em "Add New..." → "Project"
4. Clique em "Browse" e selecione a pasta do projeto
5. Clique em "Deploy"
6. Aguarde o deploy (30 segundos)
7. Seu site estará no ar com link: `nome-projeto.vercel.app`

---

### 3. **GitHub Pages**

**Vantagens:**
- Totalmente gratuito
- Integrado com GitHub
- Fácil de atualizar
- **Suporta domínio próprio gratuitamente**

**Passo a passo:**

1. Crie uma conta no [github.com](https://github.com)
2. Clique em "New repository"
3. Nome do repositório: `gabriela-telino-psicologa`
4. Marque "Public"
5. Clique em "Create repository"
6. No seu computador, abra o terminal/prompt na pasta do projeto
7. Execute os comandos:
   ```bash
   git init
   git add .
   git commit -m "Primeira versão"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/gabriela-telino-psicologa.git
   git push -u origin main
   ```
8. No GitHub, vá em "Settings" → "Pages"
9. Em "Source", selecione "main" e clique em "Save"
10. Aguarde 2-3 minutos
11. Seu site estará em: `seu-usuario.github.io/gabriela-telino-psicologa`

**Como adicionar domínio próprio no GitHub Pages:**

1. No repositório, vá em "Settings" → "Pages"
2. Em "Custom domain", digite seu domínio (ex: `gabrielatelino.com.br`)
3. Clique em "Save"
4. Marque a opção "Enforce HTTPS" (aguarde alguns minutos para ativar)
5. No seu provedor de domínio (Registro.br, HostGator, etc), configure os DNS:

**Configuração DNS para domínio próprio:**

**Opção 1 - Domínio raiz (gabrielatelino.com.br):**
- Adicione 4 registros A apontando para:
  ```
  185.199.108.153
  185.199.109.153
  185.199.110.153
  185.199.111.153
  ```
- Adicione 1 registro CNAME:
  - Nome: `www`
  - Valor: `seu-usuario.github.io`

**Opção 2 - Subdomínio (www.gabrielatelino.com.br):**
- Adicione apenas 1 registro CNAME:
  - Nome: `www`
  - Valor: `seu-usuario.github.io`

**Tempo de propagação:** 24-48 horas (geralmente funciona em 1-2 horas)

---

### 4. **Render**

**Vantagens:**
- Gratuito
- Simples
- HTTPS automático

**Passo a passo:**

1. Acesse [render.com](https://render.com)
2. Clique em "Get Started"
3. Crie uma conta (pode usar GitHub ou email)
4. Clique em "New +" → "Static Site"
5. Conecte seu repositório GitHub ou faça upload manual
6. Configure:
   - Name: `gabriela-telino`
   - Build Command: (deixe vazio)
   - Publish Directory: `.`
7. Clique em "Create Static Site"
8. Aguarde o deploy
9. Seu site estará em: `gabriela-telino.onrender.com`

---

## 🌐 Comprando um Domínio Próprio

Se quiser um domínio personalizado (ex: `gabrielatelino.com.br`):

### Onde comprar (Brasil):
- **Registro.br** - Domínios .br (mais barato, R$ 40/ano)
- **HostGator** - Vários domínios
- **GoDaddy** - Internacional
- **Hostinger** - Bom custo-benefício

### Como conectar o domínio:

**Para GitHub Pages:**
1. No repositório, vá em "Settings" → "Pages"
2. Em "Custom domain", digite seu domínio
3. Configure os DNS no seu provedor (veja instruções acima)
4. Aguarde propagação (1-48 horas)
5. Marque "Enforce HTTPS"

**Para Netlify:**
1. No painel do Netlify, vá em "Domain settings"
2. Clique em "Add custom domain"
3. Digite seu domínio
4. Siga as instruções para configurar os DNS

**Para Vercel:**
1. No projeto, vá em "Settings" → "Domains"
2. Adicione seu domínio
3. Configure os DNS conforme instruções

---

## 📱 Checklist Antes de Publicar

- [ ] Adicionar as fotos na pasta `images/`
- [ ] Testar todos os links (WhatsApp, email)
- [ ] Verificar se o mapa está funcionando
- [ ] Testar em diferentes navegadores
- [ ] Testar no celular
- [ ] Verificar se todas as seções estão corretas
- [ ] Confirmar informações de contato

---

## 🔄 Como Atualizar o Site

### Netlify:
- Arraste a pasta atualizada novamente na área de deploy
- Ou conecte com GitHub para deploy automático

### Vercel:
- Faça upload da pasta atualizada
- Ou use GitHub para atualizações automáticas

### GitHub Pages:
```bash
git add .
git commit -m "Atualização do site"
git push
```

---

## 💡 Dicas Importantes

1. **Otimize as imagens** antes de fazer upload:
   - Use ferramentas como TinyPNG ou Squoosh
   - Mantenha as imagens abaixo de 500KB cada

2. **Teste o site** antes de divulgar:
   - Abra em diferentes dispositivos
   - Teste todos os botões e links

3. **SEO Básico** (opcional):
   - Adicione meta description no HTML
   - Use títulos descritivos
   - Adicione alt text nas imagens

4. **Backup**:
   - Mantenha sempre uma cópia local dos arquivos
   - Use GitHub como backup automático

---

## 🆘 Problemas Comuns

**Site não carrega as imagens:**
- Verifique se os nomes dos arquivos estão corretos
- Certifique-se de que as imagens estão na pasta correta

**Mapa não aparece:**
- Verifique a conexão com internet
- Teste em outro navegador

**Botão do WhatsApp não funciona:**
- Confirme se o número está correto no formato internacional
- Teste o link diretamente

---

## 📞 Suporte

Se tiver dúvidas sobre hospedagem:
- Netlify: [docs.netlify.com](https://docs.netlify.com)
- Vercel: [vercel.com/docs](https://vercel.com/docs)
- GitHub Pages: [pages.github.com](https://pages.github.com)

---

**Recomendação Final:** Use o **Netlify** pela facilidade e rapidez. É perfeito para iniciantes e oferece tudo que você precisa gratuitamente!
