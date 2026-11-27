# 🧵 AmorEmRetalhos — Landing Page & Catálogo Artesanal

> Catálogo estático e landing page para a loja artesanal **AmorEmRetalhos**, especializada em colchas de retalhos (patchwork) e peças feitas à mão com tecidos 100% algodão, florais, xadrez, poá, listras e cores afetivas.

Projeto desenvolvido com **HTML5 semântico** e **CSS3 puro** (sem dependências ou frameworks pesados), totalmente responsivo (desktop, tablet e mobile) e pronto para publicação instantânea no **GitHub Pages**.

---

## 🚀 Como Publicar no GitHub Pages (Passo a Passo)

1. Envie estes arquivos para o seu repositório no GitHub:
   ```bash
   git init
   git add .
   git commit -m "feat: landing page AmorEmRetalhos completa para GitHub Pages"
   git branch -M main
   git remote add origin https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git
   git push -u origin main
   ```
2. No GitHub, acesse a aba **Settings** (Configurações) do repositório.
3. No menu lateral esquerdo, clique em **Pages**.
4. Em **Build and deployment > Branch**:
   - Selecione a branch `main` (ou `master`).
   - Mantenha a pasta como `/ (root)`.
   - Clique em **Save**.
5. Aguarde cerca de 1 a 2 minutos. O GitHub gerará o link oficial do seu site (ex: `https://seu-usuario.github.io/AmorEmRetalhos/`).

---

## ⚙️ Como Personalizar Informações

Todos os caminhos e referências utilizam caminhos relativos (`./css/style.css`, `./assets/images/...`), garantindo funcionamento perfeito em subpastas ou domínios personalizados.

### 1. Alterar o Número do WhatsApp
- **Número atual:** `+55 67 99299-9623` (código internacional: `5567992999623`).
- **Onde alterar:** No arquivo `index.html`.
- **Como encontrar:** Abra o `index.html` e pesquise por `5567992999623`. Substitua pelo seu novo número mantendo o formato `55` + `DDD` + `NÚMERO` nos links `https://wa.me/5567992999623?...`.

### 2. Alterar o E-mail de Contato
- **E-mail atual:** `amoremretalhos@gmail.com`
- **Onde alterar:** No arquivo `index.html`.
- **Como encontrar:** Pesquise por `amoremretalhos@gmail.com` e substitua no atributo `href="mailto:seu-email@dominio.com"` e no texto visível.

### 3. Substituir ou Adicionar Novas Imagens
As imagens estão armazenadas na pasta [`assets/images/`](./assets/images/):
- `colcha-king.jpg`: Imagem da Colcha King e do Hero principal.
- `colcha-queen.jpg`: Imagem da Colcha Queen Floral & Poá.
- `colcha-artesanal.jpg`: Imagem da Colcha Casal e Retalhos Tradicionais.
- `detalhe-almofadas.jpg`: Imagem de almofadas decorativas e mesa de costura artesanal.

Para atualizar uma imagem, basta colar seu novo arquivo JPG dentro de `assets/images/` com o mesmo nome, ou atualizar o atributo `src` correspondente no `index.html`.

### 4. Ajustar Medidas ou Blocos
- No arquivo `index.html`, localize os blocos `<article class="product-card">`.
- Cada produto possui uma tabela identificada com `<table class="measurements-table">` com campos fáceis de editar: tamanho da colcha, tamanho dos blocos (10x10, 15x15 ou 20x20 cm), itens inclusos e tipo de manta/forro.

### 5. Alterar Cores e Estilo Visual
- No arquivo [`css/style.css`](./css/style.css), todas as cores estão organizadas no topo no bloco `:root`:
  - `--terracotta`: Tom terracota principal.
  - `--mustard`: Mostarda acolhedora.
  - `--sage`: Verde-sálvia natural.
  - `--bg-body`: Tom creme suave / off-white do fundo.
  - `--text-main`: Cacau profundo para leitura com alto contraste acessível.

---

## 📁 Estrutura de Arquivos

```
AmorEmRetalhos/
├── index.html                   # Estrutura HTML5 semântica e acessível
├── README.md                    # Documentação e instruções de configuração
├── css/
│   └── style.css                # Estilos visuais puros, responsivos e comentados
└── assets/
    └── images/                  # Fotos de produtos otimizadas para carregamento rápido
        ├── colcha-king.jpg      # Colcha Cama King em destaque
        ├── colcha-queen.jpg     # Colcha Cama Queen floral
        ├── colcha-artesanal.jpg # Colcha Casal vibrante em patchwork
        └── detalhe-almofadas.jpg# Detalhes de blocos, costura e almofadas
```

---

## ✨ Características Técnicas & Acessibilidade

- **100% Livre de Frameworks Pesados:** Carregamento instantâneo no GitHub Pages e em redes móveis 3G/4G.
- **Tipografia Cuidadosa:** Combina *Playfair Display* (títulos com ar artesanal nobre), *Caveat* (toque caligráfico afetivo) e *Plus Jakarta Sans* (leitura limpa e agradável).
- **Direção de Arte Afetiva:** Detalhes que remetem a pespontos, costura artesanal, tons quentes e sombras suaves.
- **Microinterações:** Botão flutuante de WhatsApp, acordeão nativo de Dúvidas Frequentes (sem Javascript pesado) e menu retrátil para celulares.
- **Contraste Acessível:** Padrão WCAG AA/AAA para conforto visual de todos os públicos.
