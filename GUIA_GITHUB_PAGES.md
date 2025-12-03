# 📘 Guia: Como Publicar no GitHub Pages

## 🎯 Objetivo
Publicar o Manual de Atualização Tasy no GitHub Pages para acesso online.

---

## 📋 Passo a Passo

### 1️⃣ Criar Repositório no GitHub

1. Acesse [github.com](https://github.com)
2. Clique no botão **"+"** (canto superior direito) → **"New repository"**
3. Preencha:
   - **Repository name:** `manual-tasy` (ou nome de sua preferência)
   - **Description:** `Manual interativo para atualização do sistema Tasy EMR`
   - **Visibilidade:** 
     - ✅ **Public** (se quiser compartilhar publicamente)
     - 🔒 **Private** (se quiser manter privado)
   - ✅ Marque: **"Add a README file"** (opcional)
4. Clique em **"Create repository"**

---

### 2️⃣ Preparar Arquivos Localmente

Você já tem os arquivos prontos. Organize-os assim:

```
manual-tasy/
├── index.html              ← Seu manual completo
├── README.md               ← Documentação do projeto
└── scripts/                ← (Opcional) Pasta para scripts
    ├── desativar_jobs.sql
    └── reativar_jobs.sql
```

---

### 3️⃣ Fazer Upload dos Arquivos

**Opção A: Via Interface Web (Mais Fácil)**

1. No seu repositório recém-criado, clique em **"Add file"** → **"Upload files"**
2. Arraste os arquivos:
   - `index.html`
   - `README.md`
3. Adicione uma mensagem de commit: `Adiciona manual interativo Tasy v2.0`
4. Clique em **"Commit changes"**

**Opção B: Via Git (Linha de Comando)**

```bash
# 1. Clone o repositório (substitua seu-usuario)
git clone https://github.com/seu-usuario/manual-tasy.git
cd manual-tasy

# 2. Copie os arquivos para o diretório
# (copie index.html e README.md para esta pasta)

# 3. Adicione os arquivos
git add .

# 4. Commit
git commit -m "Adiciona manual interativo Tasy v2.0"

# 5. Push para o GitHub
git push origin main
```

---

### 4️⃣ Ativar GitHub Pages

1. No repositório, vá em **"Settings"** (Configurações)
2. No menu lateral esquerdo, clique em **"Pages"**
3. Em **"Source"** (Fonte):
   - Selecione **"Deploy from a branch"**
4. Em **"Branch"**:
   - Selecione **"main"** (ou "master")
   - Selecione **"/ (root)"**
5. Clique em **"Save"**

⏰ **Aguarde 1-3 minutos** para o site ser publicado

---

### 5️⃣ Acessar seu Manual Online

Após a publicação, você verá uma mensagem:

```
✅ Your site is live at https://seu-usuario.github.io/manual-tasy/
```

**Copie este link e acesse!** 🎉

---

## 🔧 Personalizações Opcionais

### Adicionar Domínio Customizado

1. Em **Settings → Pages**
2. Em **"Custom domain"**, digite seu domínio
3. Configure DNS conforme instruções

### Adicionar Scripts SQL Separados

Crie uma pasta `scripts/`:

```bash
mkdir scripts
# Adicione seus arquivos .sql na pasta
git add scripts/
git commit -m "Adiciona scripts SQL"
git push
```

---

## 📝 Atualizar o Manual

Sempre que fizer alterações:

**Via Web:**
1. Clique no arquivo que quer editar
2. Clique no ícone de lápis ✏️
3. Faça as alterações
4. Clique em **"Commit changes"**

**Via Git:**
```bash
# Edite os arquivos localmente
git add .
git commit -m "Atualiza manual com melhorias"
git push
```

⏰ Mudanças aparecem em 1-3 minutos

---

## 🎨 Melhorias Futuras

### Adicionar Favicon Personalizado

Crie um arquivo `favicon.ico` e coloque na raiz:

```html
<!-- Adicione no <head> do index.html -->
<link rel="icon" href="favicon.ico" type="image/x-icon">
```

### Adicionar Google Analytics (Opcional)

```html
<!-- Antes de </head> -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

---

## ✅ Checklist Final

- [ ] Repositório criado no GitHub
- [ ] Arquivos enviados (index.html e README.md)
- [ ] GitHub Pages ativado em Settings
- [ ] Site acessível via URL
- [ ] Testado em diferentes dispositivos
- [ ] README.md atualizado com URL correta
- [ ] Link compartilhado com equipe

---

## 🆘 Problemas Comuns

### Problema: Site não carrega (404)

**Solução:**
- Verifique se o arquivo se chama exatamente `index.html`
- Confirme que o GitHub Pages está ativado
- Aguarde alguns minutos após ativar

### Problema: Mudanças não aparecem

**Solução:**
- Limpe o cache do navegador (Ctrl+Shift+R)
- Aguarde 2-3 minutos
- Verifique se o commit foi feito corretamente

### Problema: CSS não carrega

**Solução:**
- Verifique se o CSS está inline no HTML (como está atualmente)
- Se usar CSS externo, verifique o caminho do arquivo

---

## 📞 Precisa de Ajuda?

- 📚 [Documentação GitHub Pages](https://docs.github.com/pages)
- 💬 [GitHub Community](https://github.community/)
- 📧 Suporte técnico via Issues do repositório

---

## 🎉 Pronto!

Seu manual agora está online e acessível de qualquer lugar!

**URL Exemplo:** `https://seu-usuario.github.io/manual-tasy/`

Compartilhe o link com sua equipe! 🚀
