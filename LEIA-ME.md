# SITE n4flow — PRONTO PARA SUBIR NA NETLIFY
## Guia rápido de deploy e personalização

---

## SUBIR O SITE (5 minutos)

1. Acesse app.netlify.com e crie conta grátis (email ou Google)
2. No painel, arraste este ZIP para a área de upload
3. Pronto! O site já está no ar com um link .netlify.app
4. Teste todas as páginas: /, /diagnostico/, /diagnostico/obrigado.html

---

## CONECTAR DOMÍNIO

1. Registre n4flow.com.br no registro.br (~R$40/ano)
2. Na Netlify: Site settings > Domain management > Add custom domain
3. Siga as instruções da Netlify para configurar DNS
4. A Netlify gera certificado SSL gratuito automaticamente

---

## PERSONALIZAR ANTES DE SUBIR

### 1. FOTOS (mais importante!)
No arquivo index.html, procure os comentários:
<!-- TROCAR POR: <img src="foto-antonio.jpg" ... -->

Para cada pessoa, faça:
- Tire/escolha uma foto profissional (400x400px, JPG)
- Salve como foto-antonio.jpg e foto-kellyn.jpg na raiz do site
- Substitua a linha do placeholder pela tag <img> indicada no comentário

### 2. LINKS
Procure href="#" e troque pelos links reais:
- LinkedIn do Antonio
- LinkedIn da Kellyn
- LinkedIn da n4flow (quando criar)
- URL do blog TheBILab (já está como https://thebilab.com/blog — ajuste se for diferente)

### 3. CALENDLY
No arquivo diagnostico/obrigado.html, troque:
https://calendly.com/SEU-LINK-AQUI/diagnostico
pelo link real do Calendly de vocês.

### 4. WHATSAPP
No arquivo diagnostico/obrigado.html, troque:
(00) 00000-0000
pelo WhatsApp real de vocês.

### 5. EMAIL
Troque contato@n4flow.com.br pelo email real quando tiverem o Google Workspace configurado.

---

## SOBRE O FORMULÁRIO

O formulário usa Netlify Forms (gratuito, nativo).
- Os dados aparecem automaticamente em: app.netlify.com > seu site > Forms
- Para receber por email: Site settings > Forms > Form notifications > Add email
- Limite: 100 envios/mês no plano grátis (mais que suficiente para começar)

---

## COMO EDITAR O SITE DEPOIS

Opção 1 (simples): Edite os arquivos .html num editor de texto, re-zipe e arraste na Netlify
Opção 2 (melhor): Conecte um repositório GitHub na Netlify — edite no GitHub e o site atualiza sozinho

---

## ARQUIVOS DO SITE

index.html .............. Página principal (home)
diagnostico/index.html .. Página do formulário de diagnóstico
diagnostico/obrigado.html Página de obrigado após envio (link para Calendly)
robots.txt .............. Configuração para buscadores e IA
404.html ................ Página de erro
_redirects .............. Config da Netlify para erros 404
