# O que é Bootstrap❓

:crystal_ball:  Bootstrap é um framework _front-end_ e de código _open source_ que permite o desenvolvimento rápido de sites responsivos com consistência de bibliotecas e comandos. É o framework _front-end_ mais utilizado pelo mundo .

:mag_right: [O que é Framework?](#framework)

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

###### Veja mais:

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