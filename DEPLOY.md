# 🚀 Guia de Publicação - GitHub Pages

## Pré-requisitos

1. **Conta no GitHub**: Se não tiver, crie em [github.com](https://github.com)
2. **Git instalado**: Você precisará instalar o Git

## 📋 Passo a Passo

### 1. Instalar o Git (se necessário)

O Git não está instalado no seu Mac. Você tem duas opções:

**Opção A - Via Xcode Command Line Tools (Recomendado)**
```bash
xcode-select --install
```
Siga as instruções na tela que aparecerá.

**Opção B - Via Homebrew**
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew install git
```

### 2. Configurar o Git (primeira vez)

Abra o Terminal e execute:
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@example.com"
```

### 3. Criar Repositório no GitHub

1. Acesse [github.com](https://github.com) e faça login
2. Clique no botão **"+"** no canto superior direito
3. Selecione **"New repository"**
4. Configure:
   - **Repository name**: `petlovers-portfolio`
   - **Description**: "Portfolio do projeto Petlovers - App de adoção de animais"
   - Marque **"Public"**
   - **NÃO** marque "Add a README file" (já criamos um)
5. Clique em **"Create repository"**

### 4. Inicializar Git no Projeto

No Terminal, navegue até a pasta do projeto e execute:

```bash
cd /Users/clarice/Documents/Projeto-vivecoding-petlovers

# Inicializar repositório Git
git init

# Adicionar todos os arquivos
git add .

# Fazer o primeiro commit
git commit -m "Initial commit: Petlovers Portfolio"

# Adicionar o repositório remoto (substitua SEU-USUARIO pelo seu username do GitHub)
git remote add origin https://github.com/SEU-USUARIO/petlovers-portfolio.git

# Renomear branch para main
git branch -M main

# Enviar para o GitHub
git push -u origin main
```

### 5. Ativar GitHub Pages

1. No GitHub, vá para o seu repositório `petlovers-portfolio`
2. Clique em **"Settings"** (Configurações)
3. No menu lateral, clique em **"Pages"**
4. Em **"Source"**, selecione:
   - Branch: `main`
   - Folder: `/ (root)`
5. Clique em **"Save"**
6. Aguarde alguns minutos

### 6. Acessar o Site Publicado

Seu site estará disponível em:
```
https://SEU-USUARIO.github.io/petlovers-portfolio/portfolio.html
```

## 🎯 Dica Importante

Para que `portfolio.html` seja a página inicial, você tem duas opções:

**Opção 1**: Renomear `portfolio.html` para `index.html`
```bash
mv portfolio.html index.html
git add .
git commit -m "Rename portfolio.html to index.html"
git push
```

**Opção 2**: Manter como está e acessar via `/portfolio.html`

## 🔄 Atualizando o Site

Sempre que fizer alterações:

```bash
git add .
git commit -m "Descrição das alterações"
git push
```

O GitHub Pages atualizará automaticamente em alguns minutos.

## ❓ Problemas Comuns

### "Git não encontrado"
- Instale o Git seguindo o passo 1

### "Permission denied"
- Configure suas credenciais do GitHub
- Considere usar SSH keys ou GitHub CLI

### "Site não carrega"
- Aguarde 5-10 minutos após o primeiro deploy
- Verifique se o GitHub Pages está ativado nas configurações

## 📞 Precisa de Ajuda?

Se encontrar algum problema, me avise que te ajudo a resolver! 🚀

---

**Próximos Passos Recomendados:**
1. Instalar o Git
2. Criar conta/repositório no GitHub
3. Seguir os comandos acima
4. Compartilhar o link do seu portfolio! 🎉
