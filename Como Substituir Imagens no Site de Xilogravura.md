# Como Substituir Imagens no Site de Xilogravura

## Guia Simplificado para Iniciantes

Este guia foi criado especialmente para quem não tem experiência com programação, mas quer personalizar o site com suas próprias imagens.

### O que você precisa saber

No site que criamos, existem **blocos cinzas** onde as imagens devem aparecer. Esses blocos são como "espaços reservados" que você pode substituir pelas suas próprias fotos.

### Passo 1: Prepare suas imagens

1. **Encontre ou tire suas fotos** das ferramentas, obras de xilogravura, etc.
2. **Salve as imagens** em formatos comuns como `.jpg`, `.png` ou `.jpeg`
3. **Dê nomes simples** para suas imagens, sem espaços ou caracteres especiais
   - ✅ Bom: `goiva-em-v.jpg`, `obra-j-borges.png`
   - ❌ Evite: `Goiva em V (nova).jpg`, `obra@jborges#1.png`

### Passo 2: Organize suas imagens

1. **Crie uma pasta** chamada `images` na mesma pasta onde estão os arquivos do site
2. **Coloque todas suas imagens** dentro desta pasta `images`

### Passo 3: Abra os arquivos para editar

Você precisará abrir os arquivos HTML em um **editor de texto**. Recomendamos:
- **Bloco de Notas** (Windows)
- **TextEdit** (Mac) 
- **Notepad++** (Windows - gratuito)
- **Visual Studio Code** (Todos os sistemas - gratuito)

### Passo 4: Encontre o bloco cinza que quer substituir

1. **Abra o arquivo HTML** da página que quer editar (ex: `historia.html`, `ferramentas.html`)
2. **Procure por** `<div class="image-placeholder"`
3. **Você verá algo assim:**

```html
<div class="image-placeholder goiva-v">
    <span>Imagem: Goiva em V</span>
</div>
```

### Passo 5: Substitua pelo código da sua imagem

**Apague** todo o bloco acima e **substitua** por:

```html
<div class="tool-image">
    <img src="images/sua-imagem.jpg" alt="Descrição da sua imagem">
</div>
```

**Exemplo prático:**
- Se sua imagem se chama `goiva-v.jpg` e mostra uma goiva em V
- Substitua `sua-imagem.jpg` por `goiva-v.jpg`
- Substitua `Descrição da sua imagem` por `Goiva em V`

**Resultado final:**
```html
<div class="tool-image">
    <img src="images/goiva-v.jpg" alt="Goiva em V">
</div>
```

### Passo 6: Salve e teste

1. **Salve o arquivo** (Ctrl+S no Windows, Cmd+S no Mac)
2. **Abra o arquivo HTML** no seu navegador (duplo clique no arquivo)
3. **Verifique** se a imagem apareceu no lugar do bloco cinza

### Exemplo Completo

**ANTES (bloco cinza):**
```html
<div class="image-placeholder goiva-v">
    <span>Imagem: Goiva em V</span>
</div>
```

**DEPOIS (com sua imagem):**
```html
<div class="tool-image">
    <img src="images/goiva-v.jpg" alt="Goiva em V">
</div>
```

### Dicas Importantes

1. **Sempre mantenha** a estrutura da pasta:
   ```
   Sua pasta do site/
   ├── index.html
   ├── historia.html
   ├── ferramentas.html
   ├── styles.css
   └── images/
       ├── goiva-v.jpg
       ├── obra-jborges.png
       └── suas-outras-imagens...
   ```

2. **Cuidado com maiúsculas e minúsculas** - `Goiva.jpg` é diferente de `goiva.jpg`

3. **Se a imagem não aparecer**, verifique:
   - O nome do arquivo está correto?
   - A imagem está na pasta `images`?
   - Você salvou o arquivo HTML depois de editar?

### Onde encontrar cada tipo de imagem no site

**Página História (`historia.html`):**
- Procure por: `china-art`, `japan-art`, `europe-art`, `brazil-art`
- Procure por: `cordel-theme`, `cultural-theme`, `masters-theme`

**Página Ferramentas (`ferramentas.html`):**
- Procure por: `goiva-v`, `goiva-u`, `facas`, `buris`
- Procure por: `matrix-mdf`, `matrix-compensado`, `matrix-linoleo`

**Página Exemplos (`exemplos.html`):**
- Procure por: `traditional-style`, `modern-style`, `experimental-style`
- Procure por: `jborges-work`, `samico-work`, `other-artists`

**Página Dicas (`dicas.html`):**
- Procure por: `simple-good`, `complex-avoid`
- Procure por: `lighting-setup`, `posture-correct`, `stable-support`

### Precisa de Ajuda?

Se algo não funcionar:
1. **Verifique** se seguiu todos os passos
2. **Teste** com uma imagem pequena primeiro
3. **Certifique-se** de que a imagem não está corrompida

Lembre-se: é normal errar algumas vezes no início. Com prática, ficará mais fácil!

