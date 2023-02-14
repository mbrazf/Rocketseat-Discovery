# HTML
<br>
<br>

### Comentários

-   Comentários no HTML
```
    <!-- -->
```
<hr>

### Anatomia das Tags

-   As Tags funcionam da seguinte forma:

```
<h1> TÍTULO </h1>
```
-   Você faz a abertura delas, coloca o nome da Tag e as fecha como no exemplo. No caso dessa Tag, seu conteúdo é a de título, juntando a abertura, fechamento e o conteúdo, teremos um Elemento HTML.

-   Há também Elementos vazios que diferente do exemplo acima não se fecha daquela forma, mas assim:
```
 <img src=" " alt=" ">
 ```
<hr>

### Atributos

-   Há também os atributos booleanos, que não precisam de conteúdo, booleano significando que apenas possuem dois tipos de valores, sendo eles verdadeiro ou falso, não havendo texto, apenas essas duas opções.

```
<input type="text" disabled>
```
-   Outro fator que devemos levar em consideração são as aspas, recomendado apenas o uso das aspas duplas, para não desencadear problemas no código.
<hr>

###  Atributos Globais

-   Atributos globais são atributos aplicáveis em todas as Tags, sendo as principais:

<br>

-   class — além de classificar as Tags, é usada para aplicar estilo css e também para acessar com o JavaScript.
```
<div class="conteúdo"></div>
```

-   contenteditable — usado para editar o conteúdo da página, porém não é mantido após salvar.
```
<div contentedtable="true"></div>
```

-   data- — usado para expandir os tipos de atributos que podemos usar para fazer mais tarde lógica no JavaScript , utilizado em css também.
```
<div data-qualquercoisaaqui=""></div>

-   Escrito com "-" ou tudo junto.
```
-   hidden — usado para esconder uma Tag.
```
<div class="carrinho" hidden>conteúdo</div>
```

-   id — usado apenas 1 por Tag para identificação, para também mais tarde usar no JavaScript e css.
```
<div id="texto">conteúdo</div>

<div id="texto2">conteúdo</div>
```

-   style — aplica a estilização na Tag, normalmente não se usa "style" dentro da Tag, mas sim em arquivos externos.
```
<div style="color: red">
```

-   tabindex — usado para ordenar o Tab na página.

```
<div tabindex="3"> </div>

<div tabindex="1"> </div>

<div tabindex="2"> </div>
```

-   title — serve para definir um título para a Tag, quando colocamos o mouse descansando em cima do conteúdo da página.
```
<div title="Definindo um título"></div>
```
<hr>

### Aninhamento Hierarquia

-   Aninhamento em HTML significa colocar uma tag dentro da outra, porém não é qualquer tag que podemos colocar dentro de outra, existe uma hierarquia por trás delas, por exemplo:
```
<p> 
    <em>texto<em>
    <p> texto2</p> 
</p>

-   Podemos ver no exemplo acima que a tag <em></em>(usada para dar enfase em um texto) é pertencente a Tag <p></p>(usada para criar um parágrafo).

-   Também é possível notar que há um fluxo, onde as tags são lidas por ordem de cima para baixo.

-   Por fim o posicionamento de elementos, podemos ver que a tag <em></em> não está em uma outra linha como na tag <p></p>, existem tags que quebram a linha, então mesmo que colocarmos a tag <p></p> uma do lado da outra, visualmente vai dar quebra de linha.
```
<hr>

### Caracteres Reservados

-   Caracteres reservado são caracteres usados no próprio HTML, como < > & " " ' ', não podemos usar nas tags, pois dão erro, mesmo aparecendo na preview o navegador vai tentar ler esses caracteres de alguma forma que faça sentido. Para usarmos precisamos troca-los por outras formas de escrever.
```
<p>
    &lt; - simbolo menor que <
    &gt; - simbolo maior que >
    &amp; - E comercial &
    <br> - quebra de linha
    &quot; - aspas  
    &apos; - apóstrofo, aspas simples
</p> 
```
<hr>

### Anatomia de um documento HTML

-   Estaremos vendo nesta aula sobre a Anatomia do documento HTML e como ver o nosso HTML, além do preview.

-   Se abrirmos o documento .html pelo navegador estaremos vendo a nossa página e se clicarmos em ver o código fonte dela, estaremos vendo o HTML que escrevemos no VSCode.

-   Agora na parte de anatomia de um documento HTML, temos este exemplo.

```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>Anatomia do Documento</title>
    </head>

    <body>
        <h1>Título</h1>
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Officiis saepe similique perferendis mollitia a assumenda doloribus omnis, quidem tempore accusamus repudiandae. Accusamus, rem dolorum ad repellendus distinctio blanditiis praesentium nulla?
        </p>
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Officiis saepe similique perferendis mollitia a assumenda doloribus omnis, quidem tempore accusamus repudiandae. Accusamus, rem dolorum ad repellendus distinctio blanditiis praesentium nulla?
        </p>
    </body>
</html>
```
-   O padrão seria esta forma.

```
<!DOCTYPE html> — diz ao navegador que estamos a trabalhar com HTML 5.

<html></html> — o próprio HTML, elemento raiz, o inicio da cadeia.

<head></head> — contém configurações importantes para página, mas não ainda o que o usuário vai ver.

<meta> — onde vai representar vários tipos de metadados da página.

<title></title> — título da página.

<body></body> — onde haverá conteúdo visual da página.
```
-   Se quiser facilitar tudo digitando ! o emmet irá completar automaticamente.
<hr>

### Criando projetos

-   Estaremos vendo como criar um projeto html.

-   Abrindo o explorador de arquivos do seu computador, indo na parte de usuário > documentos e criará a pasta do projeto, e arrastará para o VSCode.

-   Você pode criar arquivos, por exemplo: index.html, ou criar pastas.
<hr>
<br>

## Trabalhando com Elementos
<br>

### Semântica

-   Vamos falar de semântica em HTML.

-   Um dos principais objetivos é dar uma estruturação para o texto, para que haja significado e também uma melhor leitura e para isso usamos elementos semânticos, são mais de 100, mas todos muito importantes, são apenas benefícios.
<hr>

### Títulos e parágrafos

-   Nesta aula estaremos aprendendo a como fazer títulos e parágrafos, para uma melhor leitura, uma melhor semântica.
```
<h1></h1> — indo de 1 à 6 é a tag para título, 1 sendo o maior e 6 sendo o menor, a hierarquia indo de título, subtítulo e etc.

<p></p> — este sendo a tag de parágrafo.
```
<hr>

###  Listas

-   Listas no HTML são feitas da seguinte forma:

```
<li> </li> — colocar os elementos da lista. 
<ul> </ul> — para uma lista não ordenada.
<ol> </ol> — para uma lista ordenada.
```
```
<h1>Suco detox</h1>
<h2>Ingredientes:</h2>
<ul>
    <li>3 folhas de couve;</li>
    <li>1 laranjas;</li>
    <li>1 pedacinho gengibre;</li>
    <li>300 ml de água;</li>
    <li>Adoçante a gosto;</li>
    <li>Gelo a gosto.</li>
</ul>
```
<hr>

###  Citações

-   Temos o "blockquote" que é um bloco de citação que você queira deixa maior, tendo uma estilização mais diferente.
-   O "cite" é o atributo em que colocamos ou citamos o link direto no texto.
-   O "code" é um bloco onde contém códigos
-   O "q" é usado para citações curtas que não precisam de parágrafos ou quebras de linha.

```
<blockquote cite="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/blockquote">
    O <strong>Elemento HTML <code>&lt;blockquote&gt;</code> </strong> (ou <em>HTML Block
    Quotation Element</em>) indica que um texto externo foi citado.
</blockquote>

<p>De acordo com <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/blockquote">
    <cite>página MDN blockquote</cite></a>:
</p>

<p>O elemento quote — <code>&lt;q&gt;</code> — é <q cite="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/q">usado para citações curtas que não precisam de parágrafos ou quebras de linha.</q> -- <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/q">
<cite>MDN q page</cite></a>.</p>
```
<hr>

### Abreviações

-   Elemento muito comum encontrado na web é a de abreviação, mas de alguma forma queremos mostrar a palavra inteira.

```
<p>Usamos <abbr title="Hypertext Markup Language">HTML</abbr>  para estruturar nossos documentos da web.</p>
```
-   Se colocarmos o mouse em cima da abreviação, teremos a palavra inteira.
<hr>

### Detalhes de contato

```
-   A tag usada para apenas colocar detalhes de contato é a tag <address> </address>, não endereço em si, mas por exemplo o autor da página.

<address>
    <p>Mayk Brito <br>
    <strong>Campo Grande, MS</strong>
    </p>
</address>
```
<hr>

### Listas de Descrição

-   Usado para marcar uma lista de itens e suas descrições.
```
-   <dl></dl> — tag para lista de descrições.
-   <dt></dt> — tag para o termo da descrição.
-   <dd></dd> — tag para descrição.


<h2>Glossário</h2>
<dl>
    <dt>Hypertext</dt>
    <dd>É um hiper texto com possibilidades...</dd>

    <dt>Markup</dt>
    <dd>Marcação do texto</dd>

    <dt>Languague</dt>
    <dd>Linguagem com sua semântica e sintaxe....</dd>
</dl>
```
<hr>

### Representação de códigos

-   Para representar códigos usamos as tags:

```
-   <code></code> — muda a cor do conteúdo para representar código.
-   <pre></pre> — tag para criar um bloco de código, mantém os espaços em branco.

<pre>
    <code>
        &lt;
    </code>
</pre>
```
<hr>

### Elementos Genéricos

```
-   <div> </div> — tag usada para agrupar conteúdo.
-   <span> </span> — tag usada para agrupar texto, em uma ideia mais de linha.

<div class="cart">
    <span>Camiseta</span>
    <span>r$ 99,00</span>
</div>
```
<hr>

## Links

### Tag âncora

-   São os famosos hyperlinks, e a tag usada para se criar um é a 
```
<a href=" ></a>
``` 
-   responsável por ligar várias páginas.

-   Em sua anatomia ele recebe atributos globais (title, id ,class,...) e o mais importante href, a referência, podendo ser url completa, fragmento, email, telefone e mais diversos outros. 
-   há também o atributo de download, que é download="", usado junto do href="",por exemplo, se você colocar o link de uma imagem no href="" com o atributo de download, a imagem será baixada ao invés de irmos até a página e se colocarmos um valor no atributo de download, ele irá dizer como você vai salvar o arquivo.

-   Por fim temos o atributo target="", que irá dizer qual o alvo do nosso disparo, ou seja, se não tivermos o target, quando clicarmos no link, ele vai pegar o mesmo alvo, a mesma página e apenas vai trocar o conteúdo, mas se usarmos o atributo, por exemplo target="_blank", ele vai abrir uma página com o conteúdo.
<hr>

### Conteúdos dos hyperlinks

-   Estaremos vendo o que podemos colocar dentro do conteúdo do elemento a.
-   Qualquer coisa pode ser colocado, até mesmo outras tags, e mais de uma.
```
 <a href="http://google.com" title="Ir para google">
    <h1>Google</h1>
    <p>Claro que posso</p>
    <img src="https://source.unsplash.com/random" width=300 height=300 alt="">
</a>
```
-   Neste exemplo há até imagens.
<hr>

### Caminhos e URLs

-   Algo importante que precisamos saber ao criar links é como navegar neles, juntamente em como navegar no caminho dos arquivos.

-   No caso dos links são as URLs, que são sequência de texto que define onde algo está localizado na web, por exemplo https://rocketseat.com.br, ela mostrando que esse endereço levará para algum lugar da web.

-   No caso dos arquivos, são os seus caminhos, onde, no explorador de arquivos, um recurso está localizado, podendo ser imagem, pdf, qualquer arquivo basicamente, abrindo alguns arquivos do nosso projeto no VSCode, usando o elemento a, iremos escrever ao invés de https://..., apenas o nome do arquivo, o próprio VSCode possui a inteligência de saber que o arquivo está lá, lembrando que também podemos usar os atributos que usamos nas URLs.
<hr>

### Navegando pelos diretórios

```
<a href="hyperlinks.html">arquivo na pasta anterior</a>
<br>
<a href="./urls-caminhos.html">arquivo no diretório raiz</a>
<br>
<a href="urls-caminhos.html">arquivo na mesma pasta</a>
<br>
<a href="outros/conteudo-a-element.html">arquivo na pasta outros, que está na pasta anterior</a>
```
-   Para o mesmo diretório, local, raiz apenas colocamos o nome do arquivo no href.
-   Para entrar em um diretório colocamos o nome do diretório e /, como no exemplo "outros/conteudo-a-element.html"
-   Para sair de um diretório colocamos ../ ,ele sairá do diretório, semelhante a sair de uma caixa que está dentro de outro.
-   E por fim o diretório raiz especificamente, usamos apenas ./ , o próprio VSCode irá completar.
-   Caso você coloque um arquivo que não existe ou mesmo está no diretório errado, vai dar erro de não ter encontrado o arquivo.
<hr>

### Caminhos absolutos e relativos 

-   No caminho absoluto inclui-se o protocolo e o nome de domínio e sempre apontará para o mesmo local, já que é absoluto. Como por exemplo esta URL http://www.rocketseat.com.br/projeto/index.html é absoluto(mesmo não levando a lugar nenhum, é apenas um exemplo).

-   No caminho relativo, é relativo à página, pasta aberta, ou seja, se não tiver irá consequentemente dar erro, apontará para lugares diferentes. Como por exemplo apenas google.com.
<hr>
<br>

## Tabelas

-   Estaremos vendo agora sobre o elemento table, que ajuda na organização de dados, criando tabelas.

-   Prós  
        -Visualização de dados via linhas e colunas.  
        -Boa acessibilidade para leitura dos dados 
    
-   Contras  
        -Pouco flexível  
        -Precisa de estilização para melhor visualização 
        -Não usar para criar seu layout
<hr>

### Organizando Tabelas

-   Agora vamos dar uma melhor organizada na nossa tabela.

```
-   Colocaremos o nosso cabeçalho, na tag <thead></thead> e o nosso corpo no <tbody></tbody> e criaremos o rodapé usando <tfoot></tfoot> colocando os dados total.

-   Por fim poderemos colocar a tag <caption></caption> para descrever sobre o que a nossa tabela é, ficando mais ou menos assim:

<table>
    <caption>Pessoas por idade</caption>
    <thead>
        <tr>
            <th>Nome</th>
            <th>Idade</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Mayk</td>
            <td>35</td>
        </tr>
        <tr>
            <td>Diego</td>
            <td>25</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td>Total:</td>
            <td>2 Pessoas</td>
        </tr>
    </tfoot>
</table>
```
<hr>

### Tabela Básica

```
-   Para fazer uma tabela básica, apenas precisaremos da tag <table></table>, dentro dela iremos usar a tag <tr></tr>(table row) para criar uma linha na tabela, e dentro dela usaremos a tag <th></th> para o cabeçalho.

-   Depois faremos o tr novamente, só que agora não sendo o cabeçalho, e sim o td.

-   Ficará da seguinte foram:

<table>
    <tr>
        <th>Nome</th>
        <th>Idade</th>
    </tr>
    <tr>
        <td>Mayk</td>
        <td>35</td>
    </tr>
    <tr>
        <td>Diego</td>
        <td>25</td>
    </tr>
</table>
```
-   Pronto tabela básica.
<hr>

### Tabela Complexa

-   Estaremos criando uma tabela bem mais complexa, com alguns atributos a mais e uma acessibilidade a mais para tabelas complexas.

-   Faremos uma tabela que contém 2 lojas, onde estaremos vendo quantos produtos foram vendidos e produzidos e agruparemos por nome dos produtos.
<hr>

### Thead complexa

-   Veremos como fazer um thead complexo.

-   Primeiro de tudo iremos criar o nosso table, colocando a descrição com o caption.

-   Criaremos o thead para começarmos o nosso cabeçalho, abrimos o tr dentro para linha e colocamos dentro deste tr 3 th, o primeiro sendo vazio.

-   Na próxima linha já temos os produzidos e vendidos, com o auxilio do emmet, criamos direto 4 th e colocamos os produzidos e vendidos.

-   Notamos que ainda está desorganizado, então usaremos o atributo rowspan="2", na primeira linha, para ocupar 2 linhas, empurrando os elementos para o lado.

-   Agora vemos que sobrou 2 colunas vazias, então usaremos o atributo de coluna colspan="2" nas 2 lojas.
```
<table>
    <caption>Produzidos x Vendidos por Loja</caption>
	<thead>
        <tr>
            <th rowspan="2"></th>
            <th colspan="2">Afonso Pena</th>
            <th colspan="2">Antônia Pereira</th>
        </tr>
        <tr>
            <th>Produzidos</th>
            <th>Vendidos</th>
            <th>Produzidos</th>
            <th>Vendidos</th>
        </tr>
  </thead>
</table>
```
<hr>

### Tbody complexo

-   Veremos como fazer um tbody complexo.

-   Dando continuidade a nossa tabela, iremos criar o tbody, abrir uma linha com o tr, colocar o nome do produto, porém ele será um th, ou seja um cabeçalho, e com a ajuda do emmet criaremos 4 td, para colocarmos o tanto de produtos produzidos e vendidos, e repetiremos, mas para outro produto.
```
<table>
    <caption>Produzidos x Vendidos por Loja</caption>
    <thead>
        <tr>
            <th rowspan="2"></th>
            <th colspan="2">Afonso Pena</th>
            <th colspan="2">Antônia Pereira</th>
        </tr>
        <tr>
            <th>Produzidos</th>
            <th>Vendidos</th>
            <th>Produzidos</th>
            <th>Vendidos</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>Vassouras</th>
            <td>50</td>
            <td>30</td>
            <td>20</td>
            <td>20</td>
        </tr>
        <tr>
            <th>Baldes</th>
            <td>10</td>
            <td>10</td>
            <td>30</td>
            <td>25</td>
        </tr>
    </tbody>
</table>
```
<hr>

### Melhorando o aspecto com colgroup
```
-   Colocamos a tag <colgroup></colgroup>, dentro colocamos 3 <col>, onde na segunda colocamos o atibuto style="background-color: red" e na terceira style="background-color: blue", porém ainda está desorganizado por isso colocaremos span="2" para alinharmos a cor com a coluna.

<table>
    <caption>Produzidos x Vendidos por Loja</caption>
 
    <colgroup>
        <col>
        <col span="2" style="background-color: red">
        <col span="2" style="background-color: blue;">
    </colgroup>
    
    <thead>
        <tr>
            <th rowspan="2"></th>
            <th colspan="2">Afonso Pena</th>
            <th colspan="2">Antônia Pereira</th>
        </tr>
        <tr>
            <th>Produzidos</th>
            <th>Vendidos</th>
            <th>Produzidos</th>
            <th>Vendidos</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>Vassouras</th>
            <td>50</td>
            <td>30</td>
            <td>20</td>
            <td>20</td>
        </tr>
        <tr>
            <th>Baldes</th>
            <td>10</td>
            <td>10</td>
            <td>30</td>
            <td>25</td>
        </tr>
    </tbody>
</table>
```
<hr>

### Melhorando Acessibilidade

-   Estaremos usando o atributo scope, que serve permitir que essa acessibilidade saiba que o escopo do cabeçalho é relacionado com, o agrupamento, ou a coluna, ou a linha, o atributo é escrito scope="" .
```
<table>
    <caption>Produzidos x Vendidos por Loja</caption>
 
    <colgroup>
        <col>
        <col span="2" style="background-color: red">
        <col span="2" style="background-color: blue;">
    </colgroup>
    
    <thead>
        <tr>
            <th rowspan="2"></th>
            <th colspan="2" scope="colgroup">Afonso Pena</th>
            <th colspan="2" scope="colgroup">Antônia Pereira</th>
        </tr>
        <tr>
            <th scope="col">Produzidos</th>
            <th scope="col">Vendidos</th>
            <th scope="col">Produzidos</th>
            <th scope="col">Vendidos</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope="row">Vassouras</th>
            <td>50</td>
            <td>30</td>
            <td>20</td>
            <td>20</td>
        </tr>
        <tr>
            <th scope="row">Baldes</th>
            <td>10</td>
            <td>10</td>
            <td>30</td>
            <td>25</td>
        </tr>
    </tbody>
</table>
```
<hr>
<br>

## Cabeçalho

### head
```
-   <head></head> é a parte não visível pelo navegador, onde se faz configurações, contém informações como o título, links para o css, para o favicon.
```

### meta

    -   Falaremos agora sobre a tag meta , ela serve para definir metadados, como codificação de caracteres especiais e portabilidade para dispositivos mobiles.
-   Meta normalmente virá com o atributo name para especificar a meta, content para conteúdo, mas há também como o atributo charset, para caracteres especiais.
```
<head>
    <!-- codificação de caracteres especiais -->
    <meta charset="UTF-8">

    <!-- portabilidade para dispositivos mobiles -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

</head>
```

### Favicon

    -   Favicon é uma abreviação para "favorite icon", refere-se aos ícones dos favoritos a alguns anos atrás, mas nos dias de hoje acabou ficando este termo, antigamente ele era por 16 pixeis, porém com o avanço da tecnologia isso mudou.

```
Para colocarmos o ícone usaremos a tag <link> com o atributo rel="icon", que seria para representar relação, no caso a tag link vai conter um ícone, depois o href para mostrar onde está o ícone.

<!--
    <link> para ícones personalizados
-->

<!-- favicon básico -->
<link rel="icon" href="/icons/icon-48x48.png?v=cfca599cb367ccaf7377d56ddc7542f5"/>
```

### Meta SEO

-   Veremos agora das metas que são importantes para SEO(Search Engine Optimization ou motores de busca, como o google).

-   Esses já vimos anteriormente.
```
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

-   Temos também o de autor, para definir o autor da página, para possuirmos propriedade sobre a página.
```
<meta name="author" content="Mayk Brito">
```
-   Este meta é usado para descrição de sites, caso você não tenha esse meta, o navegador irá procurar qualquer texto seu, mas muito melhor escolher o que você quer que apareça.
```
<meta name="description" content="Um website para iniciantes em programação">
```

-   Esse meta diz para o robô do google o que queremos que ele faça, ele é responsável por colocar os resultados da busca , por exemplo. É possível dizer ao robô seguir links na página, através do follow, ou o contrário com o nofollow , ou "indexar" a página, através do index, ou no index.
```
<meta name="robots" content="index, follow">
```
<hr>

### Meta Social

-   Existem metadados personalizados por empresas de redes sociais, como Facebook, que criou o Open Graph, que é um tipo de metadado se quisermos colocar um tipo de conteúdo especial, caso queiramos compartilhar o link da nossa página no Facebook.

```
 <head>
    <!-- Open Graph: facebook -->
    <meta property="og:image" content="https://cdn-images-1.medium.com/max/92/1*TkXVfLTwsHdwpUEjGzdi9w@2x.jpeg">
    <meta property="og:description" content="Aqui vem um texto para ser mostrado ao compartilhar no facebook">
    <meta property="og:title" content="Um site da Rocketseat">

    <!-- twitter -->
    <meta name="twitter:title" content="Rocketseat">
</head>
```
-   São exemplos de metadados, que o Facebook procura na hora que compartilhamos a nossa página, como imagens, descrição, texto e outros.

-   O Twitter usa o atributo name diferente do Facebook que resolveu usar o property .
<hr>
<br>

