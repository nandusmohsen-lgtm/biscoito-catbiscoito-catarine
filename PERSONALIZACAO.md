# 📋 Como Personalizar o Website Biscoito Catarine

## 🖼️ ADICIONAR FOTOS DOS PRODUTOS

### Método 1: Usar URLs de Imagens (Mais Fácil)
1. Coloque suas fotos em uma pasta `/imagens` no repositório
2. No arquivo `index.html`, procure por:
```html
<div class="produto-imagem">
    <i class="fas fa-cookie"></i>
</div>
```

3. Substitua por:
```html
<div class="produto-imagem">
    <img src="imagens/produto1.jpg" alt="Nome do Produto">
</div>
```

### Método 2: Usar Links Diretos
Se as fotos estão na internet, use:
```html
<img src="https://exemplo.com/foto.jpg" alt="Nome do Produto">
```

**Adicione esta CSS ao arquivo para que as imagens se ajustem:**
```css
.produto-imagem img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}
```

---

## 📖 ADICIONAR HISTÓRIA DE COMO COMEÇOU

Na seção "Nossa História" (linha ~350), encontre:
```html
<div class="historia-texto fade-in">
    <p>Na <strong>Biscoito Catarine</strong>...
```

Substitua o texto pelos detalhes reais da sua história.

**Para adicionar foto da fábrica**, procure por:
```html
<div class="historia-imagem fade-in">
    <div class="historia-imagem-placeholder">
        <i class="fas fa-bakery"></i>
```

E substitua por:
```html
<div class="historia-imagem fade-in">
    <img src="imagens/fabrica.jpg" alt="Nossa Fábrica">
</div>
```

---

## 📍 ADICIONAR ENDEREÇO E CONTATO

Procure a seção "Contato" (linha ~700) e atualize:

```html
<div class="contato-item">
    <i class="fas fa-map-marker-alt"></i>
    <div>
        <h3>Endereço</h3>
        <p>Rua Verdadeira, 456 - Centro</p>
        <p>Seu-Município - Estado, 12345-678</p>
    </div>
</div>
```

### 📞 ATUALIZAR TELEFONE E EMAIL:
```html
<p>(11) 98765-4321</p>
<p>contato@biscoitocatarine.com.br</p>
```

### 🕐 HORÁRIO DE ATENDIMENTO:
```html
<p>Segunda a Sexta: 8h às 18h</p>
<p>Sábado: 8h às 12h</p>
```

---

## 🗺️ ADICIONAR MAPA (Google Maps)

Procure por:
```html
<div class="contato-mapa fade-in">
    <i class="fas fa-map-marked-alt"></i>
    <p style="position: absolute...">Mapa de Localização</p>
</div>
```

Substitua por:
```html
<div class="contato-mapa fade-in">
    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3..." 
            width="100%" height="100%" style="border:0; border-radius:15px;" 
            allowfullscreen="" loading="lazy"></iframe>
</div>
```

**Para gerar o código do mapa:**
1. Acesse: https://www.google.com/maps
2. Procure seu endereço
3. Clique em "Compartilhar" → "Incorporar um mapa"
4. Copie o código `<iframe>`

---

## 🍪 ADICIONAR DESCRIÇÃO DOS PRODUTOS

Cada produto tem este formato:
```html
<div class="produto-card fade-in" data-categoria="bolachas">
    <div class="produto-imagem">
        <i class="fas fa-cookie"></i>
    </div>
    <div class="produto-info">
        <span class="produto-categoria">Bolachas</span>
        <h3 class="produto-nome">Bolacha Confeitada</h3>
        <p class="produto-descricao">Deliciosas bolachas...</p>
        <span class="produto-peso">400g</span>
    </div>
</div>
```

**Para adicionar PREÇO**, insira após `<span class="produto-peso">`:
```html
<p style="color: var(--cor-terracota); font-weight: 700; margin-top: 1rem;">R$ 25,90</p>
```

---

## 📱 ADICIONAR REDES SOCIAIS

Procure por:
```html
<div class="footer-social">
    <a href="#" aria-label="Facebook"><i class="fab fa-facebook-f"></i></a>
    <a href="#" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
```

Substitua `href="#"` por seus links:
```html
<a href="https://facebook.com/biscoitocatarine" ...></a>
<a href="https://instagram.com/biscoitocatarine" ...></a>
<a href="https://wa.me/5511987654321" ...></a>
```

---

## 🖼️ ADICIONAR FOTOS NA GALERIA

Procure por:
```html
<div class="galeria-grid">
    <div class="galeria-item fade-in">
        <i class="fas fa-camera"></i>
    </div>
```

Substitua por:
```html
<div class="galeria-item fade-in">
    <img src="imagens/galeria1.jpg" alt="Nossos produtos">
</div>
```

---

## 📤 COMO ENVIAR AS MUDANÇAS

### Via GitHub (Recomendado - Mais Fácil):
1. Acesse: https://github.com/nandusmohsen-lgtm/biscoito-catbiscoito-catarine
2. Clique em "Upload files"
3. Selecione suas imagens (crie pasta `imagens/`)
4. Faça commit

### Via Terminal:
```bash
git add .
git commit -m "Adicionar fotos, endereço e informações"
git push origin main
```

---

## ✨ RESULTADO FINAL

Depois de todas as mudanças, seu site terá:
- ✅ Fotos dos produtos
- ✅ História real da empresa
- ✅ Endereço e contato atualizado
- ✅ Mapa interativo
- ✅ Preços dos produtos
- ✅ Galeria com fotos
- ✅ Links de redes sociais

**Site será atualizado automaticamente no GitHub Pages em 1-2 minutos!** 🚀
