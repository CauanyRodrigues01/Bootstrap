# Bootstrap

:crystal_ball:  Bootstrap é um framework _front-end_ e de código _open source_ que permite o desenvolvimento rápido de sites responsivos com consistência de bibliotecas e comandos. É o framework _front-end_ mais utilizado pelo mundo.

:mag_right: [O que é Framework?](#framework)

## Índice

1. [Como surgiu❓](#Como-surgiu)
2. [O que é capaz de fazer❓](#O-que-é-capaz-de-fazer)
3. [Os 3 Arquivos Primários](#Os-3-Arquivos-Primários)
4. [Como baixar no Windows❓](#Como-baixar-no-Windows)
5. [Containers responsivos com Bootstrap](#Containers-responsivos-com-Bootstrap)
6. [Imagens responsivas com Bootstrap](#Imagens-responsivas-com-Bootstrap)
7. [Texto com Bootstrap](#Texto-com-Bootstrap)
8. [Botões com Bootstrap](#Botões-com-Bootstrap)
9. [Sistema grid ou Grid Layout](#Sistema-grid-ou-Grid-Layout)

## Como surgiu❓

:bulb:  Quando os engenheiros do Twitter Jacob Thorton e Mark Otto tentaram resolver uma incompatibilidade dentro da própria equipe em 2010. Logo, perceberam a grande potencialidade que aquela ideia tinha para o mundo do desenvolvimento web e foi então que lançaram no GitHub como um software livre. Em pouco tempo, a ferramenta recebeu contribuição de inúmeros desenvolvedores de todo o planeta.

:mag_right: [O que é GitHub?](#GitHub)

## O que é capaz de fazer❓

:clipboard:  É possível criar interfaces gráficas de forma rápida e fácil, utilizando layout de Grid responsivo, criando tabelas com padrões predefinidos, figuras com estilo base, modal, botões e muito mais. A [documentação do Bootstrap](https://getbootstrap.com.br/docs/4.1/getting-started/introduction/) é riquíssima, por isso é recomendado lê-la. 

## Os 3 Arquivos Primários

São 3 arquivos principais: Bootstrap.css, Bootstrap.js, e Glyphicons

### Bootstrap.css

É um framework CSS que organiza e gerencia o layout de um site. É por meio do documento HTML que o desenvolvedor vai adicionando as funcionalidades desse arquivo na sua página.

### Bootstrap.js

É um framework JavaScript responsável pela interatividade de um site. Para não terem que sempre escrever sintaxes de JavaScript, os desenvolvedores tendem a usar jQuery.  

:mag_right: [O que é JQuery?](#JQuery)

### Glyphicons

O Bootstrap utiliza o Glyphicons que é uma extensa biblioteca de ícones vetoriais de alta qualidade.

## Como baixar no Windows❓

Existe três maneiras de adicionar o bootstrap no seu projeto:

- #### Com o BootstrapCDN

  Nessa opção, o link usado no HTML dá acesso a um arquivo CSS no servidor da empresa por meio da internet. 

  ##### Vantagens:

  - Facilidade

  ##### Desvantagens:

  - Não conseguir personalizar classes do Bootstrap;
  - Possíveis erros de comunicação com o servidor do Bootstrap

  ##### Passo a passo:

  1. Adicionar dentro da tag `<head>` do HTML o seguinte código:

     ```html
     <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
     ```

  2. Antes de fechar a tag `<body>`, adicionar o seguinte código:

     ```html
     <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js" integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49" crossorigin="anonymous"></script>
     <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>
     ```

- #### Usando CSS e JS compilado

  Basta clicar nesse [link](https://github.com/twbs/bootstrap/releases/download/v4.1.3/bootstrap-4.1.3-dist.zip) do site do Bootstrap que os arquivos serão baixados, depois, é só extrair.

  ##### Vantagens:

  - Segurabilidade

  ##### Desvantagens:

  - Dificuldade na personalização das classes do Bootstrap


- #### Usando arquivos fontes

  Vamos usar o npm para baixar e consequentemente utilizar o terminal. 

  :mag_right: [O que é npm?](#npm)

  Durante o processo, é recomendável verificar no explorador de arquivos as pastas que serão criadas.

  1. Baixe o Node.js. Clique nesse [link](https://nodejs.org/en/) para baixar.

  2. Crie uma pasta

  3. Abra o terminal e digite `cd caminhoDaPastaCriadaAnteriormente`, depois clique em `enter`

  4. Digite `npm init`, depois vai clicando em `enter`

  5. Digite `npm install bootstrap`

  6. Digite `npm install jquery`

  7. Digite `npm install popper.js`

  8. Digite `npm install -g sass`

  9. Digite `sass --watch node_modules/bootstrap/scss:node_modules/bootstrap/compiler`

     Pronto, tudo está instalado na máquina e é possível modificar as classes do bootstrap. Agora veja como usar tudo isso nos seus arquivos HTML. 
  
  10. No `<head>`  o link é direcionado para os arquivos criados na máquina:

      ```html
      <link rel="stylesheet" href="node_modules/bootstrap/compiler/bootstrap.css">
      ```
  
  11. Antes de fechar a tag `<body>`, adicionar os seguintes códigos que fazem referencia aos arquivos criados na máquina:
  
      ```html
      <script src="node_modules/jquery/dist/jquery.js"></script>
      <script src="node_modules/popper.js/dist/popper.js"></script>
      <script src="node_modules/bootstrap/dist/js/bootstrap.js"></script>
      ```

## Containers responsivos com Bootstrap

Container é um dos principais componentes do Bootstrap. É invisível e permite que o layout da pagina fique alinhado corretamente nos dispositivos. No Bootstrap todos os elementos visuais da página devem estar dentro de, pelo menos, um container.

Para usá-lo basta criar uma tag html e dentro declarar uma classe chamada `.container` ou .`container-fluid`:

- #### Classe .container

  Usado para conteúdo responsivo com largura limitada:

  ```html
  <div class="container"> ... </div>
  ```

- #### Classe .container-fluid

  Usado para conteúdo responsivo com largura fluída, ou seja, toda a largura da janela.

  ```html
  <div class="container-fluid"> ... </div>
  ```

## Imagens responsivas com Bootstrap

Para tornar as imagens responsivas usa-se a classe `.img-fluid`.

```html
<img src="..." class="img-fluid" alt="...">
```

- #### Imagens com cantos arredendados

  ```html
  <img src="..." class="rounded" alt="...">
  ```

- #### Imagens em círculo

  ```html
  <img src="..." class="rounded-circle" alt="...">
  ```

- #### Imagem em miniatura com bordas

  ```html
  <img src="..." class="img-thumbnail" alt="...">
  ```

- #### Alinhamento de imagens

  O alinhamento pode ser feito usando os outros recursos do Bootstrap, como as classes para alinhamento de texto. Mas existe a forma própria para imagem usando as seguintes classes:

  - Para direita

  ```html
  <img src="..." class="float-right" alt="...">
  ```

  - Para esquerda

  ```html
  <img src="..." class="float-left" alt="...">
  ```

  - Centrada

    mx-auto = margin:auto

    d-block = display:block

  ```html
  <img src="..." class="mx-auto d-block" alt="...">
  ```

## Texto com Bootstrap

- #### Alinhamento

  - Texto justificado

  ```html
  <p class="text-justify">...</p>
  ```

  - Alinhado à esquerda

  ```html
  <p class="text-left">...</p>
  ```

  - Alinhado à direita

  ```html
  <p class="text-right">...</p>
  ```

  - Centralizado

  ```html
  <p class="text-center">...</p>
  ```

  - Outros: `.text-sm-left`, `.text-md-left`, `.text-lg-left`, `.text-xl-left`

- #### Quebra e transbordamento de texto

  Para evitar que o texto quebre, usa-se a classe `.text-nowrap`.

  ```html
  <div class="text-nowrap"> ... </div>
  ```

  Para reduzir o texto com reticências, usa-se o `.text-truncate`

  ```html
  <div class="text-truncate"> ... </div>
  ```

## Botões com Bootstrap

A classe `.btn` foi desenhada para ser usada com o elemento `<button>`, mas pode ser usada nos elementos `<a>` ou `<input>`. Observe que os botões sempre precisam da classe `btn`. Veja alguns exemplos:

```html
<button type="button" class="btn btn-primary">Primary</button>
<button type="button" class="btn btn-secondary">Secondary</button>
<button type="button" class="btn btn-success">Success</button>
<button type="button" class="btn btn-danger">Danger</button>
<button type="button" class="btn btn-warning">Warning</button>
<button type="button" class="btn btn-info">Info</button>
<button type="button" class="btn btn-light">Light</button>
<button type="button" class="btn btn-dark">Dark</button>

<button type="button" class="btn btn-link">Link</button>
```

Para usar um botão sem backround basta modificar as classes padrões por `.btn-outline-*`, sendo * as especificações do botão, por exemplo:

```html
<button type="button" class="btn btn-outline-primary">Primary</button>
```

- #### Tamanho dos botões

  - Botão grande (`btn-lg`)

    ```html
    <button type="button" class="btn btn-primary btn-lg">Botão grande</button>
    ```

  - Botão pequeno (`.btn-sm`)

    ```html
    <button type="button" class="btn btn-primary btn-sm">Botão pequeno</button>
    ```

  - Botão que ocupa a largura do pai (`.btn-block`)

    ```html
    <button type="button" class="btn btn-primary btn-lg btn-block">Botão block-level</button>
    ```

  - Botão com estado ativo

    Não há necessidade de usar a classe no `<button>`, porque já é o padrão. Para forçar a aparência, usa-se a classe `.active` e o atributo `aria-pressed="true"`.

    ```html
    <a href="#" class="btn btn-primary active" role="button" aria-pressed="true">Link primário</a>
    ```

  - Botão com estado desativado

     usa-se o atributo booleano `disabled` em qualquer elemento `<button>`.

    ```html
    <button type="button" class="btn btn-lg btn-primary" disabled>Botão primário</button>
    ```


## Sistema grid ou Grid Layout

É um sistema de grade responsivo de 12 colunas formado pela interseção de linhas horizontais e verticais, usada para para arranjar e alinhar o conteúdo na página. 

<img src="https://miro.medium.com/max/500/1*dNUEmo5R7H6NIcvjHxoB6A.gif" style="zoom: 80%;" />

1. Como sempre, organize os elementos dentro de uma `div` com a classe `.container`; 

   ```html
   <div class="container"> ... </div>
   ```

2. Organize os elementos dentro de uma `div` com a classe `rows`que serve para envolver as colunas.

   ```html
   <div class="container">
     <div class="row">
       ...
     </div>
   </div>
   ```

3.  Agora podemos indicar o número de colunas necessárias dentro de dessa `div`, com a possibilidade de ser até 12. Ressaltando que o Bootstrap tem diferentes atributos de largura de coluna (Veja em [Parâmetros grid](#Parâmetros-grid)).

   ```html
   <div class="container">
     <div class="row">
       <div class="col-sm">
         uma coluna
       </div>
       <div class="col-sm">
         outra coluna
       </div>
     </div>
   </div>
   ```

### Parâmetros grid

A estrutura é formada primeiramente pela palalavra `col`, depois pelo prefixo do tamanho e depois pela largura de quantas colunas o elemento deve ter: 

`.col-prefixoTamanho-largura`

|                             | Extra small    | Small      | Medium     | Large      | Extra large |
| --------------------------- | -------------- | ---------- | ---------- | ---------- | ----------- |
| Prefixo em classe           | `.col-`        | `.col-sm-` | `.col-md-` | `.col-lg-` | `.col-xl-`  |
| Largura máxima do container | Não tem (auto) | 540px      | 720px      | 960px      | 1140px      |



###### Saiba mais:

- #### Framework:
  

:mag_right:  É um conjunto de códigos prontos que são disponibilizados na comunidade para serem usados por outros desenvolvedores. O intuito do uso desses pacotes é aplicar características, comandos e estruturas já prontas para garantir qualidade no projeto e produtividade. Para saber mais clique [aqui](https://rockcontent.com/br/blog/framework/).

- #### JQuery:

:mag_right:  É uma plataforma de código _open source_ popular que permite adicionar várias funcionalidades em um site.  Para saber mais clique [aqui](https://www.hostinger.com.br/tutoriais/o-que-e-jquery).

- #### GitHub:

:mag_right:  É um sistema de gerenciamento de projetos e versões de códigos assim como uma plataforma de rede social criado para desenvolvedores. Para saber mais clique [aqui](https://www.hostinger.com.br/tutoriais/o-que-github).

- #### NPM:

:mag_right:  O NPM é uma ferramenta do [Node.js](https://rockcontent.com/blog/node-js/) para o gerenciamento de pacotes. Ele permite instalar, desinstalar e atualizar dependências em uma aplicação por meio de uma simples instrução na linha de comando. Para saber mais clique [aqui](https://rockcontent.com/br/blog/npm/).

###### Fonte:

- [Documentação do Bootstrap](https://getbootstrap.com.br/docs/4.1/getting-started/introduction/)

- [O Que é Bootstrap? Guia para Iniciantes](https://www.hostinger.com.br/tutoriais/o-que-e-bootstrap)  

- [O Que é Bootstrap e Para Que Serve?](https://www.ciawebsites.com.br/sites/o-que-e-bootstrap/)

- [O que é Bootstrap: Tudo sobre este Framework](https://www.homehost.com.br/blog/tutoriais/o-que-e-bootstrap/)