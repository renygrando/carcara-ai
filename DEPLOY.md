# 🚀 Guia de Deploy - GitHub Pages

## Status Atual

✅ Código completo da landing page criado
✅ Workflow de deploy automático configurado
✅ Branch `claude/carcara-landing-page-011CUuBRXtcE1P7wtMRqNyzr` no GitHub

---

## 📋 Passo a Passo para Ativar o Site

### **1. Acesse as Configurações do Repositório**

Abra no navegador:
```
https://github.com/renygrando/carcara-ai/settings/pages
```

Ou navegue manualmente:
- Vá para: https://github.com/renygrando/carcara-ai
- Clique em **Settings** (⚙️)
- No menu lateral esquerdo, clique em **Pages**

---

### **2. Configure o Source (Fonte)**

Na seção **Build and deployment**:

1. Em **Source**, selecione: **GitHub Actions**

   _(Não selecione "Deploy from a branch", selecione "GitHub Actions")_

2. Clique em **Save** (se houver botão)

---

### **3. Execute o Deploy**

Depois de configurar, o deploy pode acontecer de 2 formas:

**Opção A: Automático** (Recomendado)
- O workflow já está configurado para rodar automaticamente
- Vá para: https://github.com/renygrando/carcara-ai/actions
- Clique no workflow **"Deploy to GitHub Pages"**
- Clique em **"Run workflow"** > **"Run workflow"**

**Opção B: Trigger manual**
- Faça qualquer pequena mudança no repositório via GitHub interface
- Ou aguarde - o workflow pode iniciar automaticamente

---

### **4. Aguarde o Deploy (1-3 minutos)**

1. Acompanhe em: https://github.com/renygrando/carcara-ai/actions
2. Você verá um workflow rodando com ícone amarelo 🟡
3. Quando ficar verde ✅, o deploy está completo!

---

### **5. Acesse Seu Site! 🎉**

Seu site estará disponível em:

```
https://renygrando.github.io/carcara-ai
```

---

## 🔧 Solução de Problemas

### O workflow não está rodando?

1. Verifique se selecionou **"GitHub Actions"** (não "Deploy from a branch")
2. Vá em **Settings** > **Actions** > **General**
3. Certifique-se de que **"Allow all actions and reusable workflows"** está selecionado
4. Em **Workflow permissions**, selecione **"Read and write permissions"**
5. Salve as configurações

### Deploy falhou?

1. Vá para: https://github.com/renygrando/carcara-ai/actions
2. Clique no workflow que falhou
3. Verifique os logs de erro
4. Geralmente o problema é permissão - siga os passos acima

### Página não carrega?

1. Aguarde 2-3 minutos após o deploy verde ✅
2. Limpe o cache do navegador (Ctrl+Shift+R)
3. Tente acessar em uma aba anônima

---

## 🌐 Domínio Customizado (Opcional)

Se quiser usar **carcara.ai** em vez de **renygrando.github.io/carcara-ai**:

### 1. Configure no GitHub

1. Vá em: https://github.com/renygrando/carcara-ai/settings/pages
2. Em **Custom domain**, adicione: `carcara.ai`
3. Marque **Enforce HTTPS**
4. Clique em **Save**

### 2. Configure no seu DNS (onde comprou o domínio)

Adicione estes registros DNS:

**Para usar `carcara.ai` (sem www):**
```
Tipo: A
Host: @
Valor: 185.199.108.153

Tipo: A
Host: @
Valor: 185.199.109.153

Tipo: A
Host: @
Valor: 185.199.110.153

Tipo: A
Host: @
Valor: 185.199.111.153
```

**Para usar `www.carcara.ai`:**
```
Tipo: CNAME
Host: www
Valor: renygrando.github.io
```

### 3. Aguarde propagação DNS (pode levar até 48h)

Verifique a propagação em: https://dnschecker.org

---

## 🔄 Atualizações Futuras

Sempre que você fizer mudanças no código:

1. Faça commit e push das alterações
2. O workflow rodará automaticamente
3. Em 1-3 minutos seu site estará atualizado!

---

## 📞 Precisa de Ajuda?

Se tiver algum problema, me avise! Estou aqui para ajudar.

---

**Desenvolvido com ❤️ para Carcará**
