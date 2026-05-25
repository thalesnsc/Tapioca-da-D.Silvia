# Projeto Website - Tapioca da D.Silvia

Bem-vindo! Aqui está o projeto base para seu website de restaurante.

## 📁 Estrutura de Arquivos

```
projeto/
├── index.html      (página principal)
├── style.css       (estilos)
├── assets/         (pasta para imagens)
└── README.md       (este arquivo)
```

## 🎨 Como Personalizar

### 1. **Informações do Restaurante**
No arquivo `index.html`, procure por `[Seu Endereço]`, `[Seu Telefone]`, etc., e substitua pelos dados reais:

- **Nome do Restaurante**: Linha ~5 (título da página)
- **Logo/Emoji**: Linha ~24 (você pode trocar o emoji 🍽️)
- **Endereço**: Seção "Sobre" e "Contato"
- **Telefone**: Seção "Sobre" e "Contato"
- **Horário**: Seção "Sobre"
- **Redes Sociais**: Links no final da seção "Contato"

### 2. **Cardápio**
Edite a seção `<!-- Menu -->` (linhas ~77-110) para adicionar/remover/editar pratos:

```html
<div class="menu-item">
    <h3>Nome do Prato</h3>
    <p>Descrição do prato</p>
    <span class="price">R$ XX,XX</span>
</div>
```

### 3. **Cores**
Para mudar as cores do site, edite o arquivo `style.css`:

- **Cor principal (roxo)**: Procure por `#667eea` e troque
- **Cor secundária**: Procure por `#764ba2` e troque
- **Background**: Procure por `#1a1a1a` para a barra superior

### 4. **Adicionar Imagens**
1. Crie uma pasta `assets/` no mesmo nível do `index.html`
2. Coloque suas imagens lá (ex: `assets/prato1.jpg`)
3. Para adicionar uma imagem no menu, altere:

```html
<div class="menu-item">
    <img src="assets/nome-da-imagem.jpg" alt="Descrição">
    <h3>Nome do Prato</h3>
    <p>Descrição do prato</p>
    <span class="price">R$ XX,XX</span>
</div>
```

E adicione este CSS no `style.css`:

```css
.menu-item img {
    width: 100%;
    height: 200px;
    object-fit: cover;
    border-radius: 8px 8px 0 0;
    margin: -1.5rem -1.5rem 1rem -1.5rem;
}
```

## 🚀 Como Abrir o Site

1. Abra o arquivo `index.html` em qualquer navegador (duplo clique)
2. Ou use um servidor local:
   - **Python**: `python -m http.server 8000`
   - **Node.js**: `npx http-server`

Depois acesse: `http://localhost:8000`

## 📝 Próximos Passos

- [ ] Substituir informações do restaurante
- [ ] Editar cardápio com seus pratos
- [ ] Adicionar imagens dos pratos (pasta `assets/`)
- [ ] Atualizar links de redes sociais
- [ ] Testar responsividade no celular
- [ ] Considerar domínio e hospedagem

## 💡 Dicas de Personalização

1. **Fonte**: Para mudar a fonte, edit `font-family` em `style.css`
2. **Espaçamento**: Aumente/diminua `padding` e `margin` conforme necessário
3. **Sombras**: Customize as `box-shadow` para um visual único
4. **Ícones**: Use emojis ou adicione uma biblioteca como Font Awesome

---

**Pronto para personalizar seu website! 🎉**
