## HTML

### 1. Introdução
- **HyperText Markup Language** (Linguagem de Marcação de Hipertexto) em 1991 TIM Berners-Lee criou essa linguagem de marcação para melhorar a comunicação entre eles e seus colegas de trabalho no CERN, desde então já surgiram 5 versões e o HTML se tornou a base da web.
- Com o HTML definimos o significado e a estrutura do conteúdo da web e além de texto, nossas páginas precisam de imagens, videos e vários outros formatos e para isso temos os elementos HTML.
- "Hipertexto" refere-se a links que conectam páginas da web umas às outras, seja dentro de um único site ou entre sites.

### 2. **HTML - Básico**
- A primeira linha do documento deve ser o **`<!DOCTYPE html>`**, apesar de parecer um elemento HTML ela apenas diz oa navegador que ele está lidando com um arquivo do tipo HTML5.
- **Semântica** - Nos permite descrever mais precisamente o nosso conteúdo, agora um bloco de texto não é apenas uma div, agora é um article e tem mais significado assim. E temos vários elementos para ressignificar as divs:
**`<section>`** - Representa uma seção genérica de conteúdo quando não houver um elemento mais específico para isso.
**`<header>`** - É o cabeçalho da página ou de uma seção da página e normalmente contém logotipos, menus, campos de busca.
**`<article>`** - Representa um conteúdo independente e de maior relevância dentro de uma página, como um post de blog, uma notícia em uma barra lateral ou um bloco de comentários. Um article pode conter outros elementos, como header, cabeçalhos, parágrafos e imagens.
**`<aside>`** - É uma seção que engloba conteúdos relacionados ao conteúdo principal, como artigos relacionados, biografia do autor e publicidade. Normalmente são representadas como barras laterais.
**`<footer>`** - Esse elemento representa o rodapé do conteúdo ou de parte dele, pois ele é aceito dentro de vários elementos, como article e section e até do body. Exemplos de conteúdo de um `<footer>` são informações de autor e links relacionados.

### 3. **HTML - Elementos**
- Um elemento HTML é formado pela tag de abertura e seus atributos, o conteúdo e uma tag de fechamento. Com esses elementos podemos agrupar tipos de conteúdo, alterar tamanho e forma de fontes e adicionar diferentes mídias a nossa página web.
- **`<html>`** - A tag html é a raiz do seu documento, todos os elementos HTML devem estar dentro dela. E nela nós informamos ao navegador qual é o idioma desse nosso documento, através do atributo lang, para o português brasileiro usamos pt-BR.
- **`<head>`** - A tag head contém elementos que serão lidos pelo navegador, como os metadados - um exemplo é o charset, que é a codificação de caracteres e a mais comum é a UTF-8, o JavaScript com a tag script, o CSS através das tags style e link.
- **`<body>`** - Dentro da tag body colocamos todo o conteúdo visível ao usuário: textos, imagens, vídeos.

### 4. HTML - Atributos
- Elementos em HTML possuem atributos; são valores adicionais que configuram os elementos ou ajustam seu comportamento de várias maneiras para atender aos critérios que os usuários desejam.

### 5. HTML - Meta Tags
- A **`<meta>`** tag define metadados sobre um documento HTML. Metadados são dados (informações) sobre dados. `<meta>` tags sempre vão dentro do elemento `<head>` e normalmente são usadas para especificar o conjunto de caracteres, descrição da página, palavras-chave, autor do documento e configurações da janela de visualização.

### 6. HTML - Paragrafos
- O **`<p>`** representa um parágrafo, mas ele não suporta apenas texto, podemos adicionar imagens, código, vídeos e vários outros tipos de conteúdo dentro dele.

### 7. HTML - Titulos
- **`<h1>` - `<h6>`** - Eles não foram criados na versão 5 do HTML e nem são específicos para semântica, mas servem para esse propósito. São utilizados para marcar a importância dos títulos, sendo `<h1>` o mais importante e `<h6>` o menos. Use apenas um `<h1>` por página, pois ele representa o objetivo da sua página.

### 8. HTML - Links
- **`<area>`** - O elemento HTML define uma área dentro de um mapa de imagem que possui áreas clicáveis ​​predefinidas. Um mapa de imagem permite que áreas geométricas em uma imagem sejam associadas a um link de hipertexto `<area>`. Este elemento é usado apenas dentro de um `<map>` elemento.
- **`<link>`** - O elemento HTML especifica relacionamentos entre o documento atual e um recurso externo. Esse elemento é mais comumente usado para vincular a folhas de estilo , mas também é usado para estabelecer ícones de site (ícones de estilo "favicon" e ícones para a tela inicial e aplicativos em dispositivos móveis), entre outras coisas.
- **`<a>`** - que significa anchor/âncora, ele representa um hyperlink, é ele que interliga vários conteúdos e páginas na web. O elemento a tem vários atributos, o href e o target por exemplo. O href representa o hyperlink para onde sua âncora aponta, pode ser uma página ou de outro site, um e-mail e até mesmo um telefone, os dois últimos precisam dos prefixos mailto: e tel:, respectivamente.
O target neste momento vai servir para nos ajudar a abrir nossos links em outra aba do navegador usando o valor _blank. Exemplo: **`<a href="mailto:seu@email.com" target="_blank">seu@email.com</a>`**

### 9. HTML - Div/Span
- **`<div>`** - O elemento HTML é o contêiner genérico para conteúdo de fluxo. Ele não tem efeito sobre o conteúdo ou layout até que seja estilizado de alguma forma usando CSS (por exemplo, o estilo é aplicado diretamente a ele, ou algum tipo de modelo de layout como Flexbox é aplicado ao seu elemento pai).
- **`<span>`** - O elemento HTML é um contêiner inline genérico para conteúdo de fraseado, que não representa nada inerentemente. Ele pode ser usado para agrupar elementos para fins de estilo (usando os atributos ou ) ou porque eles compartilham valores de atributos. Deve ser usado somente quando nenhum outro elemento semântico for apropriado.

### 10. HTML - Classes
- A classe é representada de forma parecida do ID, mas é precedida por um ponto em vez do hash.
E a diferença mais importante entre eles é a forma como devem ser usados: o ID só pode ser usado uma vez em uma página HTML enquanto a classe não tem restrições.

### 11. HTML - ID
- É representado pelo símbolo # (hash) seguido de um nome para esse ID. Só pode ser usada 1 vez.

### 12. HTML - Imagens
- A web também é feita de imagens e para representá-las temos o elemento **`<img>`**, ele é um daqueles elementos sem tag de fechamento.
O elemento img é bem simples, contendo apenas 2 atributos próprios, o src e o alt.
O src é obrigatório e guarda o caminho para a imagem que você quer mostrar na página.
O alt não é obrigatório mas é altamente recomendado por melhorar a acessibilidade, ele mostra a descrição da imagem caso ela não carregue e leitores de tela usam esse atributo para descrever a imagem para o usuário saber o que ela significa.

### 13. HTML - Formularios
- **`<form>`** - O elemento HTML representa uma seção do documento contendo controles interativos para o envio de informações.
 
### 14. HTML - Input
- **`<input>`** - Tag especifica um campo de entrada onde o usuário pode inserir dados. Com diferentes entradas de dados.

### 15. HTML - Tabelas
- Uma tabela é um conjunto estruturado de dados composto de linhas e colunas ( dados tabulares ). Uma tabela permite pesquisar de forma rápida e fácil valores que indicam algum tipo de conexão entre diferentes tipos de dados, por exemplo, uma pessoa e sua idade, ou um dia da semana, ou o horário de uma piscina local.
- O conteúdo de cada tabela é delimitado por esta tag: **`<table>`** .
- O menor contêiner dentro de uma tabela é uma célula de tabela, que é criada por um **`<td>`** elemento ('td' significa 'dados da tabela').
- **`<tr>`** elemento ('tr' significa 'linha da tabela').

### 16. HTML - Listas
- **`<ul>`, `<ol>` e `<li>`** - Listas servem para agrupar uma coleção de itens, como uma lista de ingredientes ou uma lista com contatos.
O elemento **`<ul>`** cria uma lista não ordenada, onde a ordem dos elementos não é importante, e é representada com pontos, círculos ou quadrados.
O **`<ol>`** serve para criar lista ordenadas, nessas a ordem importa, portanto elas são representadas com números, algarismos romanos ou letras.
E o elemento li é um item dentro de uma dessas listas. Um **`<li>`** pode conter vários tipos de conteúdos, como parágrafos, imagens e até outras listas.


## CSS
### 1. Introdução
- Após a criação do HTML a necessidade de formatar as páginas ficou evidente, assim, em 1994, foi criada por Hakon Lie a linguagem de estilo que conhecemos por CSS (Cascading Style Sheets), é o código que estiliza o conteúdo da web.

### 2. CSS Básico
- CSS descreve como os elementos devem ser renderizados na tela, no papel, na fala ou em outras mídias.
- Quando estamos criando o layout de um site o navegador representa cada elemento HTML  como uma caixa retangular, isso é o box-model. E com CSS nós alteramos a aparência dessa caixa (largura, altura, cor de fundo, etc.). Essa caixa é composta por 4 áreas: o conteúdo, o padding, a borda e a margem.

### 3. CSS Sintaxe
- O Objetivo básico da linguagem de folhas de estilo em cascata (CSS) é permitir que um motor do navegador pinte elementos na página com características específicas como cores, posições, ou decorações. A sintaxe CSS reflete estes objetivos e seus blocos de contrução básicos são:
A **propriedade** é um identificador que possui um nome legível, que define o que será considerado ou editado.
O **valor** descreve como o recurso será tratado pelo motor. Cada propriedade possui um conjunto de valores válidos, definida por uma gramática formal, bem como um significado semântico, implementado para o motor do navegador.

### 4. CSS Seletores
- Os Seletores definem quais são os elementos de um conjunto de regras CSS para aplicação.
- São usados ​​para "encontrar" (ou selecionar) os elementos HTML que você deseja estilizar.
- **Seletor de tags** - Este seletor escolhe todos os elementos que pertencem ao nome escolhido. Exemplo: input corresponderá a qualquer elemento `<input>`.
- **Seletor por classe** - O seletor de classe seleciona elementos HTML com um atributo de classe específico. Para selecionar elementos com uma classe específica, escreva um caractere ponto (.), seguido do nome da classe. Exemplo: .class
- **Seletor por ID** - Este seletor nós escolhemos pelo valor do atributo id. Deve existir apenas um elemento com o mesmo ID no mesmo documento. Exemplo: #toc corresponderá ao elemento que possui o id=toc (definido por um atributo id="toc", ou similar).
- **Seletores Universais** - O seletor universal (*) seleciona todos os elementos HTML na página.

### 5. CSS Fonte
- **`font-family`** - Com o font-family podemos alterar a fonte dos nossos textos, como uma fonte da internet ou uma que esteja instalada no nosso computador.
- **`font-size`** - O font-size nos ajuda a mudar o tamanho do texto, existem algumas unidades de medida para ele.
- **`font-style`** - Usamos o font-style para tornar um texto itálico, por exemplo, na maioria das vezes você usará apenas o valor italic para ele, mas se precisar tirar o itálico de um texto você pode usar o valor normal.

### 6. CSS Padding
- O padding é um espaçamento entre as bordas e o conteúdo, a diferença para as margens é que declarações de imagem de fundo funcionam nele.

### 7. CSS Margin
- As margens (margin) são espaçamentos entre elementos.

### 8. CSS Display
- Uma propriedade CSS display especifica o tipo de caixa de renderização usada por um elemento. No HTML, os padrões da propriedade display são feitos a partir do comportamento descrito nas especificações HTML ou da folha de estilo padrão do navegador/usuário.

### 9. CSS Bordas
- A propriedade border pode ter 3 valores: a largura, a cor e o estilo, mas existem algumas particularidades nisso. A largura pode ser usada com várias unidades, como px, em e mm. A cor pode ser atribuída pelo nome ou por um código hexadecimal e o estilo é representada por palavras-chave, algumas delas:
**solid:** mostra uma borda simples e reta;
**dotted:** são bolinhas com um pequeno espaçamento entre elas;
**ashed:** forma uma linha tracejada.
- E se não quiser usar a propriedade border existem as propriedade específicas para cada aspecto de uma borda, são elas **`border-width`** para a largura, **`border-color`** para a cor e **`border-style`** para o estilo.
- O **`border-radius`**, ele permite arredondar os cantos de um elemento. Podemos usar várias unidades, mas as mais comuns são os pixels e a porcentagem.

### 10. CSS Unidades (Medidas)
|Comprimentos absolutos|Descrição|
|:-:|:-:|
|cm|Centímetro|
|mm|Milímetro|
|in|Polegada|
|px|Pixel|
|pt|Ponto|
|pc|Peça|

|Comprimentos relativos|Descrição|
|:-:|:-:|
|em|Em relação ao tamanho da fonte do elemento (2em significa 2 vezes o tamanho da fonte atual)|
|ex|Em relação à altura x da fonte atual (raramente usada)|
|ch|Relativo à largura do "0" (zero)|
|rem|Relativo ao tamanho da fonte do elemento raiz|
|vw|Relativo a 1% da largura da janela de visualização|
|vh|Relativo a 1% da altura da janela de visualização|
|vmin|Relativo a 1% da dimensão menor da janela de visualização|
|vmax|Relativo a 1% da dimensão maior da janela de visualização|
|%|Em relação ao elemento pai|

### 11. CSS Larguras e Alturas (min/max)
- **Width** - Largura
- **`max-widt`h** é usada para definir a largura máxima de um elemento.
- **`min-width`** - Propriedade define a largura mínima de um elemento.
- **Height** - Altura
- **`max-height`**  é usada para definir a altura máxima de um elemento.
- **`min-height`** - Propriedade define a altura mínima de um elemento.
- **auto** - Este é o padrão. O navegador calcula a altura e a largura.

### 12. CSS Variaveis
- **var()** - Função é usada para inserir o valor de uma variável CSS.
- As variáveis ​​CSS têm acesso ao DOM, o que significa que você pode criar variáveis ​​com escopo local ou global, alterar as variáveis ​​com JavaScript e alterar as variáveis ​​com base em consultas de mídia.
- Uma boa maneira de usar variáveis ​​CSS é quando se trata das cores do seu design. Em vez de copiar e colar as mesmas cores repetidamente, você pode colocá-las em variáveis. Exemplo: `var(--name, value)`

### 13. CSS Links
- Os links podem ter estilos diferentes dependendo do estado em que estão. Os quatro estados de links são:
- **`a:link`** - Um link normal e não visitado
- **`a:visited`** - Um link que o usuário visitou
- **`a:hover`** - Um link quando o usuário passa o mouse sobre ele
- **`a:active`** - Um link no momento em que é clicado

### 14. CSS FlexBox
[**FlexBox**](https://marina-ferreira.github.io/tutorials/css/flexbox/)

### 15. CSS Grid
[**Grid**](https://www.origamid.com/projetos/css-grid-layout-guia-completo/)

### 16. CSS Efeito de texto
- **text-overflow** - Especifica como o conteúdo estourado que não é exibido deve ser sinalizado ao usuário. Pode ser recortado (**clip**) u pode ser renderizado como reticências (...)(**ellipsis**)..
- **word-wrap** - Permite que palavras longas possam ser quebradas e colocadas na próxima linha.
- **word-break** - Especifica as regras de quebra de linha. (**keep-all** ou **break-all**)
- **writing-mode** - Especifica se as linhas de texto são dispostas horizontalmente ou verticalmente.

### 17. CSS !important
- **!important** - Regra em CSS é usada para adicionar mais importância a uma propriedade/valor do que o normal.
- Na verdade, se você usar a !importantregra, ela substituirá TODAS as regras de estilo anteriores para essa propriedade específica nesse elemento!

### 18. CSS Media Query
- **`@media`** - Regra é usada em consultas de mídia para aplicar estilos diferentes para diferentes tipos/dispositivos de mídia.
- Também pode ter diferentes folhas de estilo para diferentes mídias, como esta:
<br>`<link rel="stylesheet" media="screen and (min-width: 900px)" href="widescreen.css">`
<br>`<link rel="stylesheet" media="screen and (max-width: 600px)" href="smallscreen.css">`

### 19. CSS Overflow
- Propriedade especifica o que deve acontecer se o conteúdo ultrapassar a caixa de um elemento. Especifica se o conteúdo deve ser recortado ou adicionado barras de rolagem quando o conteúdo de um elemento é muito grande para caber em uma área especificada.
`overflow: visible|hidden|clip|scroll|auto|initial|inherit`

### 20. CSS Z-Index
- **`z-index`** - Propriedade especifica a ordem de pilha de um elemento (qual elemento deve ser colocado na frente ou atrás dos outros). Quando os elementos são posicionados, eles podem se sobrepor a outros elementos.
