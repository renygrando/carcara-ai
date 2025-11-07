# Carcará - Landing Page

Landing page profissional para a **Carcará**, consultoria especializada em Vendas e Inteligência Artificial.

## 🚀 Sobre o Projeto

Esta landing page foi desenvolvida para apresentar os serviços da Carcará, destacando sua expertise em transformar resultados comerciais através da combinação de estratégias de vendas comprovadas com tecnologias de IA de ponta.

## ✨ Características

### Design
- **Moderno e Profissional**: Layout clean focado em conversão
- **Responsivo**: Funciona perfeitamente em todos os dispositivos (desktop, tablet, mobile)
- **Animações Suaves**: Transições e efeitos que melhoram a experiência do usuário
- **Cores**: Gradiente azul (#3B82F6) e verde (#10B981) transmitindo confiança e crescimento

### Seções

1. **Hero Section**
   - Proposta de valor clara
   - CTAs estratégicos
   - Estatísticas de resultados

2. **Serviços**
   - 6 cards de serviços detalhados
   - Destaque para o serviço mais popular
   - Lista de features por serviço

3. **Diferenciais**
   - 6 diferenciais competitivos
   - Layout numerado para fácil leitura
   - Animações ao hover

4. **Resultados/Depoimentos**
   - Casos de sucesso reais
   - Métricas de resultados
   - Informações dos clientes

5. **Formulário de Contato**
   - Validação em tempo real
   - Formatação automática de telefone
   - Feedback visual ao enviar

6. **Footer**
   - Links para serviços e páginas
   - Redes sociais
   - Informações de contato

### Funcionalidades

- ✅ Navegação mobile responsiva
- ✅ Scroll suave entre seções
- ✅ Botão "Voltar ao topo"
- ✅ Validação de formulário
- ✅ Formatação automática de telefone
- ✅ Notificações de sucesso/erro
- ✅ Animações ao scroll
- ✅ Performance otimizada

## 🛠️ Tecnologias

- **HTML5**: Estrutura semântica
- **CSS3**: Design moderno com Grid e Flexbox
- **JavaScript (Vanilla)**: Interatividade sem dependências
- **Google Fonts**: Tipografia Inter

## 📁 Estrutura de Arquivos

```
carcara-ai/
├── index.html          # Estrutura da página
├── styles.css          # Estilos e design
├── script.js           # Interatividade e validações
└── README.md           # Documentação
```

## 🚀 Como Usar

### Opção 1: Abrir Localmente

1. Clone ou baixe este repositório
2. Abra o arquivo `index.html` em qualquer navegador moderno
3. Pronto! A página está funcionando

### Opção 2: Deploy

#### Vercel
```bash
npm i -g vercel
vercel
```

#### Netlify
```bash
npm i -g netlify-cli
netlify deploy
```

#### GitHub Pages
1. Faça push do código para o GitHub
2. Vá em Settings > Pages
3. Selecione a branch e pasta
4. Acesse sua página em `username.github.io/carcara-ai`

## 🎨 Personalização

### Cores

Edite as variáveis CSS em `styles.css`:

```css
:root {
    --primary: #3B82F6;        /* Azul principal */
    --secondary: #10B981;      /* Verde secundário */
    --dark: #0F172A;           /* Texto escuro */
    --gray: #64748B;           /* Texto secundário */
}
```

### Conteúdo

Todos os textos podem ser editados diretamente no arquivo `index.html`.

### Formulário

Para integrar o formulário com seu backend, edite a função de submit em `script.js`:

```javascript
// Linha ~95 em script.js
contactForm.addEventListener('submit', async (e) => {
    e.preventDefault();

    const formData = {
        name: document.getElementById('name').value,
        email: document.getElementById('email').value,
        phone: document.getElementById('phone').value,
        company: document.getElementById('company').value,
        message: document.getElementById('message').value
    };

    // Substitua por sua integração
    const response = await fetch('YOUR_ENDPOINT', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify(formData)
    });
});
```

### Integrações Sugeridas

- **Email**: Formspree, EmailJS, SendGrid
- **CRM**: HubSpot, RD Station, Pipedrive
- **Analytics**: Google Analytics, Hotjar, Microsoft Clarity
- **Chat**: Intercom, Drift, Crisp

## 📱 Responsividade

A landing page é totalmente responsiva e foi testada em:

- ✅ Desktop (1920px+)
- ✅ Laptop (1024px - 1919px)
- ✅ Tablet (768px - 1023px)
- ✅ Mobile (320px - 767px)

## ⚡ Performance

- Sem dependências externas (exceto Google Fonts)
- CSS otimizado com variáveis
- JavaScript vanilla (sem frameworks pesados)
- Imagens otimizadas (quando adicionadas)
- Lazy loading preparado

## 🔧 Próximas Melhorias

- [ ] Adicionar imagens otimizadas
- [ ] Implementar blog/artigos
- [ ] Criar página de cases detalhados
- [ ] Adicionar chat ao vivo
- [ ] Implementar A/B testing
- [ ] Adicionar vídeo de apresentação
- [ ] Criar versão em inglês

## 📞 Suporte

Para dúvidas ou sugestões sobre a landing page:

- Email: contato@carcara.ai
- WhatsApp: +55 11 99999-9999

## 📄 Licença

© 2024 Carcará. Todos os direitos reservados.

---

**Desenvolvido com ❤️ para transformar vendas através da IA**
