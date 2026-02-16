# 👟 SyntaxWear - E-commerce de Sapatos

Uma landing page moderna e responsiva de um e-commerce de sapatos premium, desenvolvida com HTML5, CSS3 e design por componentes.

## 📋 Visão Geral

**SyntaxWear** é uma plataforma de e-commerce especializada em sapatos de qualidade, oferecendo uma experiência de compra elegante e intuitiva. A página é totalmente responsiva e otimizada para dispositivos móveis, tablets e desktops.

### Características Principais
- ✨ Design moderno e minimalista com paleta roxa/púrpura
- 📱 Totalmente responsivo (mobile-first)
- 🎯 Menu hamburguer para dispositivos pequenos
- 🖼️ Grid dinâmico para exibição de produtos
- 🎨 Categorias de produtos: Casual, Esporte, Moderno e Futurista
- 📧 Seção de newsletter e redes sociais
- 🔗 Navegação intuitiva com links estruturados
- ⚡ Transições suaves e efeitos hover interativos

---

## 📁 Estrutura do Projeto

```
📦 E-commerce-SyntaxWear
├── 📄 index.html                # Arquivo principal HTML
├── 📄 README.md                 # Documentação do projeto
├── 📂 assets/
│   ├── 📂 css/
│   │   ├── reset.css            # CSS Reset (Andy Bell Modern Reset)
│   │   ├── base.css             # Estilos base e componentes botões
│   │   ├── header.css           # Estilos do cabeçalho e navegação
│   │   ├── hero.css             # Seção hero principal
│   │   ├── category.css         # Seção de categorias de produtos
│   │   ├── grid.css             # Grid de produtos em destaque
│   │   └── footer.css           # Rodapé com links e inscrição
│   └── 📂 images/
│       ├── 📂 icons/            # Ícones (logo, menu, redes sociais)
│       ├── 📂 hero/             # Imagem de fundo da seção hero
│       ├── 📂 categorias/       # Imagens das 4 categorias
│       ├── 📂 grid-images/      # Imagens para o grid de produtos
│       ├── 📂 produtos/         # Imagens de produtos específicos
│       └── 📂 banners/          # Banners promocionais
```

---

## 🎨 Estrutura HTML

### 1. **Header (Cabeçalho)**
- Logo da marca (SyntaxWear)
- Navegação central com 3 opções: Masculino, Feminino, Outlet
- Menu direito com: Nossas Lojas, Sobre, Perfil, Ajuda, Carrinho
- Menu hamburguer responsivo para mobile

### 2. **Main (Conteúdo Principal)**

#### Seção Hero
- Banner com fundo de imagem
- Texto destaque "Krypton One"
- CTA (Call-to-Action) com dois botões: "Ver modelos" e "Comprar"

#### Seção de Categorias
4 cartões com as linhas de produtos:
- **Casual**: Para uso do dia a dia relaxado
- **Esporte**: Para atividades físicas
- **Moderno**: Design contemporâneo e elegante
- **Futurista**: Estilo inovador e futurista

#### Seção Grid
Layout responsivo com:
- **Featured**: Destaque "Krypton One - Estilo urbano com atitude"
- **Highlight**: Tênis Preto Azul
- **Primary**: Tênis Roxo Verde
- **Model**: Foto de modelo
- **Secondary**: Tênis Colorido e Tênis Branco

### 3. **Footer (Rodapé)**
- **Seção de Contato**: Input para email, ícones de redes sociais
- **Links Principais**: 5 colunas com categorias de navegação
  - Masculino
  - Feminino
  - Outlet
  - Nossas Lojas
  - Sobre
- **Copyright**: Direitos autorais

---

## 🎭 Arquivos CSS Explicados

### **reset.css**
- CSS Reset baseado no moderno reset do Andy Bell
- Remove margins e paddings padrão
- Define box-sizing border-box
- Configura comportamentos padrão para imagens, vídeos e links

### **base.css**
- Define fonte global (Ubuntu)
- Estilos do componente `.btn` (outline e filled)
- Configuração de main com max-width de 1440px
- Efeitos hover para botões
- Media query para padding em telas menores

### **header.css**
- Cabeçalho fixo no topo com z-index 999
- Navegação flexível com gaps e alinhamentos
- Menu hamburguer (hidden por padrão, visível em 1100px)
- Hover effects com cor roxa (#9856ef)
- Responsivo para diferentes breakpoints

### **hero.css**
- Seção hero com altura de 500px
- Background image com cover
- Conteúdo centralizado à direita (end)
- Typography com letter-spacing
- Flexbox para layout dos botões

### **category.css**
- 4 cartões em flex row com gap de 30px
- Cada cartão com imagem de fundo e overlay escuro
- Botões centralizados com overlay
- Responsive em 780px com flex-wrap

### **grid.css**
- CSS Grid com 4 colunas e 3 linhas
- Grid areas: featured, highlight, primary, model, secondary-top, secondary-bottom
- Cada item com background-image diferente
- Responsive em 700px com 2 colunas e 6 linhas
- Conteúdo centralizado com absolute positioning

### **footer.css**
- Background escuro (#333333)
- Flex layout para distribuição de seções
- 5 colunas de links em grid
- Input de email com estilo customizado
- Transições suaves para hover estados
- Responsive com padding flexível

---

## 🎯 Componentes Reutilizáveis

### Botões
```css
.btn              /* Estilo base com 160px de largura */
.btn-outline      /* Transparente com borda branca */
.btn-filled       /* Fundo branco com texto roxo */
```

### Overlay
```css
.overlay          /* Sombra escura sobre imagens */
```

### Cartões
```css
.card             /* Container para categorias */
.grid-item        /* Item do grid de produtos */
```

---

## 📱 Responsividade

| Breakpoint | Comportamento |
|---|---|
| **1350px** | Reduz margin-left do nav-center |
| **1100px** | Mostra menu hamburguer |
| **1000px** | Reduz padding do main |
| **780px** | Categorias em flex-wrap |
| **700px** | Grid muda para 2 colunas |

---

## 🚀 Como Usar

### Instalação
1. Clone o repositório
```bash
git clone <repository-url>
cd E-commerce-SyntaxWear
```

2. Abra o arquivo `index.html` em seu navegador
```bash
# Windows
start index.html

# macOS
open index.html

# Linux
xdg-open index.html
```

3. Ou use um servidor local (Live Server VS Code)
- Instale a extensão Live Server
- Clique direito em index.html
- Selecione "Open with Live Server"

---

## 🎨 Paleta de Cores

| Cor | Código | Uso |
|---|---|---|
| Roxo Principal | `#6329A2` | Hover, acentos |
| Roxo Secundário | `#9856ef` | Links hover |
| Branco | `#fff` | Elementos principais |
| Cinza Escuro | `#333333` | Footer, texto primário |
| Cinza Claro | `#EDEDED` | Texto alternativo |
| Cinza Neutral | `#dedede` | Texto hero |

---

## 📐 Layout Responsivo

### Desktop (1440px+)
- Header com navegação completa
- Grid de produtos com 4 colunas
- Todas as categorias em uma linha

### Tablet (780px - 1440px)
- Menu hamburguer em ≤1100px
- Grid parcialmente responsivo
- Categorias começam a envolver em 780px

### Mobile (<780px)
- Menu hamburguer principal
- Categorias em coluna única
- Grid reduzido para 2 colunas
- Ajustes de padding e margin

---

## 🔧 Tecnologias Utilizadas

- **HTML5**: Semântica e estrutura
- **CSS3**: 
  - Flexbox para layouts
  - Grid para produtos
  - Media queries para responsividade
  - Transições e transformações
- **Fonts**: Google Fonts (Roboto, Ubuntu)
- **Imagens**: PNG, JPG (background-images)

---

## 📝 Notas Importantes

- O menu hamburguer é apenas visual (CSS only) - seria necessário JavaScript para funcionalidade completa
- Todos os links estão como `#` - precisam ser conectados a páginas reais
- As imagens são referenciadas em URLs - certifique-se de que todas existem em seus respectivos diretórios
- O projeto usa Google Fonts, requer conexão com internet

---

## 👨‍💻 Desenvolvimento

Para adicionar novos produtos ao grid:
1. Adicione a imagem em `assets/images/grid-images/`
2. Crie um novo `.grid-item` com classe específica
3. Defina `background-image` no CSS

Para adicionar novas categorias:
1. Crie um novo `.card` com classe temática
2. Adicione a imagem em `assets/images/categorias/`
3. Configure o background-image no CSS

---

## 📄 Licença

Este projeto é um exercício de programação. Sinta-se livre para usar como referência ou base para seus próprios projetos.

---

**Última atualização**: 16 de fevereiro de 2026 
