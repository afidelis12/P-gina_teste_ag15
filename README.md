# Portfólio Profissional

**Aluno:** João da Silva
**Curso:** Desenvolvimento de Sistemas

---

## Descrição do portfólio

Este projeto é um portfólio acadêmico de página única (*one page*), criado para apresentar o perfil profissional do aluno, as tecnologias estudadas e os projetos desenvolvidos ao longo do curso de Desenvolvimento de Sistemas.

A página é dividida em seções, acessadas pelo menu de navegação fixo no topo:

- **Carrossel de abertura:** três imagens em destaque logo no início da página.
- **Perfil:** foto, nome, formação, localização, área de interesse, objetivo e as tecnologias e ferramentas utilizadas.
- **Projetos:** três cartões com imagem, título, descrição e botão "Ver projeto".
- **Contato:** botões para e-mail, GitHub e LinkedIn.
- **Rodapé:** direitos autorais e informação sobre as tecnologias do site.

O layout é **responsivo**: adapta-se a computadores, tablets e celulares.

---

## Tecnologias utilizadas

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=flat-square&logo=bootstrap&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222222?style=flat-square&logo=githubpages&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)

| Ícone | Tecnologia | Uso no projeto |
|:---:|---|---|
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" width="24" height="24" alt="HTML5"> | **HTML5** | Estrutura e organização do conteúdo da página |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" width="24" height="24" alt="CSS3"> | **CSS3** | Ajustes de estilo personalizados (altura e enquadramento das imagens do carrossel) |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bootstrap/bootstrap-original.svg" width="24" height="24" alt="Bootstrap"> | **Bootstrap 5.3.3** | Layout responsivo (grid), navbar, cartões, botões e carrossel |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/devicon/devicon-original.svg" width="24" height="24" alt="Devicon"> | **Devicon** | Ícones das tecnologias na seção de perfil |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width="24" height="24" alt="Python"> | **Python** | Tecnologia estudada e apresentada no portfólio (projeto "Sistema em Python") |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" width="24" height="24" alt="Git"> | **Git** | Controle de versão do código |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="24" height="24" alt="GitHub"> | **GitHub e GitHub Pages** | Armazenamento do projeto e publicação do site na internet |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" width="24" height="24" alt="VS Code"> | **VS Code** | Editor de código utilizado no desenvolvimento |

---

## Link do site publicado

🔗 **https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/**

> Substitua `SEU-USUARIO` pelo seu usuário do GitHub e `NOME-DO-REPOSITORIO` pelo nome do seu repositório.

---

## Estrutura do projeto

```
NOME-DO-REPOSITORIO/
├── index.html
├── README.md
└── imagens/
    ├── slide1.png
    ├── slide2.png
    ├── slide3.png
    ├── perfil.png
    ├── p1.png
    ├── p2.png
    └── p3.png
```

---

## Como o projeto funciona

O projeto é um único arquivo `index.html`, que carrega o Bootstrap, o Devicon e o JavaScript do Bootstrap por meio de links de CDN (`cdn.jsdelivr.net`). Por isso, não é preciso instalar nada: basta abrir o arquivo no navegador, com internet.

O funcionamento por seção:

1. **Menu de navegação (navbar):** fica fixo no topo da tela (`sticky-top`). Os links usam âncoras (`#perfil`, `#projetos`, `#contato`), que levam o usuário direto à seção correspondente. Em telas pequenas, o menu vira um botão "hambúrguer" que abre e fecha o menu.
2. **Carrossel:** exibe três imagens da pasta `imagens/` em sequência, com troca automática.
3. **Perfil:** usa o sistema de grid do Bootstrap (`row` e `col-lg-4` / `col-lg-8`). A foto fica à esquerda e os textos e cartões de informação à direita. Em telas pequenas, os blocos ficam um abaixo do outro. Os ícones das tecnologias vêm do Devicon (por exemplo, `devicon-html5-plain`).
4. **Projetos:** três cartões (`card`) lado a lado em telas grandes, dois por linha em telas médias e um por linha no celular. Todos têm a mesma altura (`h-100`) e o botão fica sempre alinhado na parte de baixo do cartão.
5. **Contato:** cartão central com botões de e-mail (`mailto:`), GitHub e LinkedIn. Os links externos abrem em uma nova aba (`target="_blank"`).
6. **Rodapé:** faixa escura com o ano e a informação sobre as tecnologias usadas.

---

## Recurso novo adicionado: carrossel de imagens

Foi adicionado ao portfólio um **carrossel de imagens** (slideshow) na parte superior da página, logo abaixo do menu. Ele exibe três imagens grandes que se alternam automaticamente, com efeito de **transição suave (fade)**.

O recurso traz:

- troca automática dos slides;
- botões de **anterior** e **próximo** nas laterais;
- **indicadores** (bolinhas) na parte de baixo, que mostram em qual slide o usuário está e permitem ir direto a qualquer um deles;
- imagens que ocupam quase toda a altura da tela, causando um impacto visual na abertura do site.

---

## Como o recurso foi implementado

O carrossel foi criado com o componente **Carousel do Bootstrap 5**, combinando HTML, classes do Bootstrap e um pequeno trecho de CSS.

### 1. Estrutura HTML

O contêiner principal recebe o `id` do carrossel e as classes que ativam o componente:

```html
<div id="carouselPortfolio" class="carousel slide carousel-fade" data-bs-ride="carousel">
```

- `carousel slide`: define o componente e a animação de transição.
- `carousel-fade`: troca o deslizamento lateral por um efeito de esmaecimento (fade).
- `data-bs-ride="carousel"`: inicia a troca automática dos slides assim que a página carrega.

### 2. Slides

Cada imagem fica dentro de um `carousel-item`, dentro de `carousel-inner`. Apenas o primeiro recebe a classe `active`, que indica qual imagem aparece primeiro:

```html
<div class="carousel-inner">
    <div class="carousel-item active">
        <img src="imagens/slide1.png" class="d-block w-100" alt="Slide 1">
    </div>
    <div class="carousel-item">
        <img src="imagens/slide2.png" class="d-block w-100" alt="Slide 2">
    </div>
    <div class="carousel-item">
        <img src="imagens/slide3.png" class="d-block w-100" alt="Slide 3">
    </div>
</div>
```

As classes `d-block w-100` fazem a imagem ocupar toda a largura do carrossel. As imagens são carregadas da pasta `imagens/`, por caminho relativo.

### 3. Indicadores

Cada botão da área `carousel-indicators` aponta para o carrossel (`data-bs-target`) e para a posição de um slide (`data-bs-slide-to`, que começa em 0):

```html
<button type="button" data-bs-target="#carouselPortfolio" data-bs-slide-to="0" class="active"></button>
<button type="button" data-bs-target="#carouselPortfolio" data-bs-slide-to="1"></button>
<button type="button" data-bs-target="#carouselPortfolio" data-bs-slide-to="2"></button>
```

### 4. Botões anterior e próximo

```html
<button class="carousel-control-prev" type="button" data-bs-target="#carouselPortfolio" data-bs-slide="prev">
    <span class="carousel-control-prev-icon"></span>
</button>
<button class="carousel-control-next" type="button" data-bs-target="#carouselPortfolio" data-bs-slide="next">
    <span class="carousel-control-next-icon"></span>
</button>
```

O atributo `data-bs-slide="prev"` ou `"next"` indica a direção em que o carrossel deve avançar.

### 5. CSS personalizado

Para que o carrossel ocupe quase toda a tela e as imagens não fiquem distorcidas, foi escrito este CSS no `<head>`:

```css
.carousel-item {
    height: 95vh;
}
.carousel-item img {
    height: 100%;
    object-fit: cover;
}
```

- `height: 95vh`: o carrossel ocupa 95% da altura da janela do navegador.
- `object-fit: cover`: a imagem preenche toda a área, sendo cortada se necessário, sem esticar nem deformar.

### 6. JavaScript

Nenhum código JavaScript precisou ser escrito. O comportamento (troca automática, botões e indicadores) é feito pelo arquivo `bootstrap.bundle.min.js`, carregado no final da página:

```html
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
```

Ele lê os atributos `data-bs-*` do HTML e ativa o carrossel automaticamente.

---

## Como publicar este projeto (GitHub Pages)

1. Envie o `index.html`, o `README.md` e a pasta `imagens` para o repositório no GitHub.
2. No repositório, acesse **Settings → Pages**.
3. Em **Source**, escolha **Deploy from a branch**.
4. Selecione a branch **main** e a pasta **/ (root)**, e clique em **Save**.
5. Aguarde de 1 a 3 minutos. O endereço do site aparecerá no topo da página de configuração do Pages.

---

## Autor

**João da Silva** — Desenvolvimento de Sistemas
