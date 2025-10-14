# Comandos Git para Windows - Passo a Passo

## 📋 Pré-requisitos

1. **Instalar o Git:**
   - Baixe em: https://git-scm.com/download/win
   - Execute o instalador
   - Use as opções padrão (Next, Next, Install)

2. **Criar conta no GitHub:**
   - Acesse: https://github.com
   - Clique em "Sign up"
   - Crie sua conta

---

## 🚀 Comandos para Subir o Projeto (COPIE UM POR VEZ)

### Passo 1: Abrir o Prompt de Comando na pasta do projeto

1. Abra o Explorador de Arquivos
2. Navegue até: `C:\Users\Josue\OneDrive\Documentos\landing_page_Gabi`
3. Na barra de endereço, digite `cmd` e pressione Enter
4. O Prompt de Comando abrirá na pasta correta

---

### Passo 2: Executar os comandos (UM DE CADA VEZ)

**Comando 1:** Inicializar o repositório Git
```
git init
```
Pressione Enter e aguarde.

---

**Comando 2:** Adicionar todos os arquivos
```
git add .
```
Pressione Enter e aguarde.

---

**Comando 3:** Fazer o primeiro commit
```
git commit -m "Primeira versao"
```
Pressione Enter e aguarde.

---

**Comando 4:** Renomear a branch para main
```
git branch -M main
```
Pressione Enter e aguarde.

---

**Comando 5:** Conectar com o GitHub
```
git remote add origin https://github.com/SEU-USUARIO/gabriela-telino-psicologa.git
```
⚠️ **IMPORTANTE:** Substitua `SEU-USUARIO` pelo seu nome de usuário do GitHub!

Exemplo: Se seu usuário é "joaosilva", o comando fica:
```
git remote add origin https://github.com/joaosilva/gabriela-telino-psicologa.git
```

Pressione Enter e aguarde.

---

**Comando 6:** Enviar os arquivos para o GitHub
```
git push -u origin main
```
Pressione Enter.

⚠️ **Vai pedir login:**
- Username: seu usuário do GitHub
- Password: use um **Personal Access Token** (não é a senha normal!)

---

## 🔑 Como Criar Personal Access Token

O GitHub não aceita mais senha normal. Você precisa criar um token:

1. No GitHub, clique na sua foto (canto superior direito)
2. Vá em **Settings**
3. No menu lateral, role até o final e clique em **Developer settings**
4. Clique em **Personal access tokens** → **Tokens (classic)**
5. Clique em **Generate new token** → **Generate new token (classic)**
6. Dê um nome: "Landing Page"
7. Marque a opção: **repo** (todas as sub-opções)
8. Role até o final e clique em **Generate token**
9. **COPIE O TOKEN** (você só verá uma vez!)
10. Use esse token como senha quando o Git pedir

---

## 📝 Resumo dos Comandos (Copie e Cole UM POR VEZ)

```
git init
```

```
git add .
```

```
git commit -m "Primeira versao"
```

```
git branch -M main
```

```
git remote add origin https://github.com/SEU-USUARIO/gabriela-telino-psicologa.git
```

```
git push -u origin main
```

---

## ✅ Depois de Enviar

1. Vá no GitHub
2. Entre no repositório `gabriela-telino-psicologa`
3. Clique em **Settings** (no menu do repositório)
4. No menu lateral, clique em **Pages**
5. Em **Source**, selecione **main**
6. Clique em **Save**
7. Aguarde 2-3 minutos
8. Seu site estará em: `seu-usuario.github.io/gabriela-telino-psicologa`

---

## 🔄 Para Atualizar o Site Depois

Quando fizer mudanças nos arquivos:

```
git add .
```

```
git commit -m "Atualizacao do site"
```

```
git push
```

---

## 🆘 Erros Comuns

**Erro: "git não é reconhecido"**
- Você precisa instalar o Git: https://git-scm.com/download/win
- Reinicie o Prompt de Comando após instalar

**Erro: "remote origin already exists"**
- Execute: `git remote remove origin`
- Depois execute novamente o comando do remote add

**Erro ao fazer push (pede senha)**
- Use o Personal Access Token, não a senha normal
- Veja as instruções acima de como criar o token

---

## 💡 Alternativa Mais Fácil

Se os comandos Git parecerem complicados, use o **Netlify**:

1. Acesse: https://www.netlify.com
2. Faça login
3. Arraste a pasta `landing_page_Gabi` inteira
4. Pronto! Site no ar em 30 segundos

Netlify é MUITO mais fácil e também é gratuito!
