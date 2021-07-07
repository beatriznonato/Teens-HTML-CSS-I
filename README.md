# Teens HTML & CSS I

Turma Teens { Reprograma }| Online | Fundamentos de HTML e CSS. 

Plano de aula desenvolvido para a <b>primeira semana</b> do curso. As aulas vão acontecer nos dias 03 (sábado) e 06 (quarta-feira) de julho 2021.

## Client-side and Server-Side

Para desenvolvimento web existem dois tipos de linguagens: as linguagens <b>client-side</b> e as linguagens <b>server-side</b>.
- As linguagens <b>client-side</b> são linguagens onde apenas o seu <i>navegador</i> vai entender. O responsável por processar essa linguagem é o browser (Google Chrome,
Safari, Firefox...)
- As linguagens <b>server-side</b> são linguagens que o <i>servidor</i> entende. Isso quer dizer que será escrito um código que o servidor vai processar e então enviar
para o seu navegador a resposta.
<div align="center">
  <img alt="computador enviando imagem de um gato pro servidor" src="https://thumbs.gfycat.com/CloudySaneIcelandichorse.webp" width="400">
</div>

O <b>cliente</b> é todo meio que eu uso pra acessar sites e sistemas a partir de um endereço web (www).

Um exemplo prático disso é eu precisar encontrar a foto de um gatinho. Através do meu computador eu vou fazer pesquisar "foto de gatinho".
O navegador vai <b>enviar</b> essa informação que eu coloquei lá na caixinha de pesquisa para o <b>servidor</b> do Google, que é um computador que pode estar em qualquer 
lugar do mundo e que tem armazenado essa informação e a resposta do servidor para o navegador vai ser a foto do gatinho.

Assim, os profissionais que trabalham na interface do usuário, são chamados de <b>Desenvolvedores front-end</b>, e aqueles que trabalham no core da aplicação, 
fazendo uma programação que somente o servidor irá entender são chamados de <b>Desenvolvedores back-end</b>.
<div align="center">
  <img alt="imagem com um notebook e ao lado um datacenter" src="https://www.datocms-assets.com/14946/1590690600-front-end-back-end-1080x608.png?auto=format&w=1080" width="350">
  <img alt="imagem de um gatinho na boia, em cima ceu limpo, embaixo da boia tentaculos, roda e remo" src="https://248006.selcdn.ru/main/upload/setka_images/7e62b3835daf60768398349b17d2a465e65aadd7.png" width="320">
</div>

- As linguagens client-side são HTML, CSS e JAVASCRIPT

Onde o HTML é responsavél pela <b>estrutura</b> da página, o CSS pela <b>estilização</b> e o JavaScript pela <b>interação</b>.

<div align="center">
  <img alt="imagem do deadpool caveira, com cores e se mexendo" src="https://moz-static.moz.com/youmoz_uploads/javascript-seo/5948abfc0e2df5.02876591.gif" width="500">
</div>

Nessas duas primeiras semanas iremos focar em <b>HTML & CSS</b>. 

#### A estrutura de pastas básicas é:

> O index.html é o padrão da Web de ser o primeiro arquivo processado pelo navegador, geralmente é usado como Home da página, por isso é criado na raiz do projeto e para o css o padrão é criar um arquivo nomeado de style.css uma pasta img para guardar as imagens.

<hr>
<div align="center">
  <img alt="logo hmtl na cor laranja" src="https://logodownload.org/wp-content/uploads/2016/10/html5-logo-8.png" width="100">
</div>

## HTML
  HTML é abreviação de <b>Hyper Text Markup Language</b> é uma linguagem de marcação que usa uma sintaxe especial para descrever a estrutura de uma página da web para o navegador. Ou seja, não é uma linguagem de programação, pois não tem lógica (algoritmos).
  
<div align="center"> 
<img alt="tela na cor azul mostrando escrita HTML e transita para tag" src="https://i.pinimg.com/originals/15/d5/4d/15d54d9da034f969e0711f031bf43ea9.gif" width="320">
</div>

- Tag

A maiora dos elementos ```<html>``` possui uma tag de abertura e uma tag de fechamento.
As tags de **abertura** têm a seguinte aparência:
``` html
<h1>
```
As tags de **fechamento** têm a seguinte aparência:
``` html
</h1>
```
Há exceções de Tags que não precisam de um fechamento somente a Tag de abertura, como é o caso do ```<meta>```,```<link>``` e ```<img>```.

Por convenção, todas as tags HTML são escritas em minúsculas, exemplo:
``` html
 <p> </p> 
```

Toda tag é um elemento ```<html>```

### Estrutura

A estrutura do HTML:
``` html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```
- Doctype 

O Document Type Defination (DTD, ou simplesmente Doctype) é uma instrução que informa ao navegador qual é a especificação do código que está sendo usada no documento, e deve ser declarado antes do elemento ```<html>```.

- Elemento ```<html>```

Na árvore de elementos do código, o elemento principal é  ```<html>```, que comporta todos os outros elementos filhos.
``` html
<html lang="pt-br">
```
É no elemento ```<html>``` que declaramos o idioma principal do documento

### Head

- Elemento ```<head>```
Metadados ficam contidos no elemento ```<head>```. 

Os Metadados são um conjunto de informações a respeito da página e do conteúdo nela publicado. Essas informações são usadas pelos navegadores e user-agents em geral, sendo invisíveis para os usuários.

- Elemento ```<title>```

O elemento ```title``` também vai dentro do ```<head>```, mas com a função de ser usada pelos mecanismos de busca para montar uma [SERP](https://rockcontent.com/br/blog/serp/).

- Elemento ```<link>```

Com o elemento ```<link>``` podemos referenciar documentos que serão usados em nossa página. O atributo <i>rel</i> indica o tipo de documento que está sendo referenciado, como por exemplo o **rel=”stylesheet”** fazendo referência à folha de estilo CSS usadas para formatar a página.
``` html
<link rel="stylesheet" type="text/css" href="/sidecode/style.css">
```

- Charset

A metadata Charset é usada para indicar a [codificação de caracteres](https://pt.wikipedia.org/wiki/Codifica%C3%A7%C3%A3o_de_caracteres) que a nossa página está utilizando. No exemplo abaixo, estamos indicando uma codificação de caracteres do tipo:
``` html
<meta charset="utf-8">
```

### Body

- Elemento ```<body>```

O ```<body>``` localizado no mesmo nível do ```<head>```, este elemento representa o conteúdo principal da página. Aqui estão localizados todos os comandos necessários para a criação do documento HTML.

- Elemento ```<div>```

O elemento ```<div>``` representa um bloco de texto. Os outros elementos possuem regras de utilização bem definidas. Caso seja necessário a criação de um bloco de texto que não se encaixe em alguma regra defina de bloco, pode-se utilizar o recurso da ```<div>```.
``` html
  <div>
    Eu sou uma div !
  </div>
```

- Títulos

Os elementos **h1** são frequentemente usados para **títulos principais**, enquanto os elementos **h2** são geralmente usados para **subtítulos**. Existem também elementos h3, h4, h5 e h6 para indicar diferentes níveis de subposições.
``` html 
<h1> Sou um titulo! </h1>
```

- Parágrafo

Os elementos **p** são os elementos usados para **texto de parágrafo** em sites. p é a abreviatura de "parágrafo".
``` html 
<p> Sou um parágrago </p>
```

## HTML5

  HTML5 fornece elementos HTML com estrutura mais descritivas (semânticas), facilitando a leitura. Isso inclui: 
- ```main```, 
- ```header```, 
- ```footer```, 
- ```nav```, 
- ```article```, 
- ```section``` e outros.

Esses elementos ajudam na **otimização do mecanismo de pesquisa (SEO) e na acessibilidade**.

- Cabeçalho com o elemento ```<header>```

O elemento ```<header>``` do HTML5 é usado para definir o cabeçalho de uma página, e pode conter logo, títulos entre outros.
``` html
<header>
   <img alt="logo" src="/img/logo.png">
   <h1>Entendo a estrutura e semântica do HTML5</h1>
</header>
```

- Navegação Global com o elmento ```<nav>```

O elemento ```<nav>``` é utlizado para agrupar uma lista de links para outras partes do site, seja essa lista de navegação interna ou externa.
``` html
<nav>
       <ul class="menu">
           <li><a href="inicio.html">Início</a></li>
           <li><a href="quem-somos.html">Quem somos</a></li>
           <li><a href="servicos.html">Serviços</a></li>
           <li><a href="contato.html">Contato</a></li>
       </ul>
</nav>
```
  
- Conteúdo principal com o elemento ```<main>```

Esse é um dos principais elementos semânticoss do HTML5. É responsável por definir o principal conteúdo da página, que deve ser exclusivo para o documento.
O ```<main>``` não deve conter nenhum conteúdo a ser replicado em documentos como logotipos de sites, formulários de pesquisa, links de navegação e barras laterais.
Sendo o elemento principal, não deve ser aninhado dentro de ```header```, ```footer```, ```section``` e outros. Deve estar situado no ```body```.

- Diferentes seções com o elemento ```<section>```

O elemento ```<section>``` representa uma seção genérica dentro de um documento. Esse elemento pode conter um agrupamento de textos com vários capítulos, seções numeradas entre outros.
``` html
<section>
  <h1>Titulo da seção</h1>
  <p>Primeiro parágrafo da seção</p>
</section>
<section>
  <h1>Titulo da segunda seção</h1>
  <p>Segundo parágrafo da seção</p>
</section>
```

- O conteúdo central com o elemento ```<article>```

O elemento ```<article>``` serve para identificar um conteúdo independente e de maior relevância dentro da página, que pode ser distribuido via feed, como um post, artigo ou bloco de comentários.
O elemento ```<article>``` pode conter outros elementos como ```<header>``` ou ```<footer>```.
``` html
<article>
   <header>
       <h1>Entendendo o elemento Article</h1>
       <p>Publicado em <time pubdate datetime="2011-09-01">01 de Setembro de 2011</time></p>
   </header>
   ...conteúdo...
   <footer>
       <small>© Todos os direitos reservados.</small>
   </footer>
</article>
```

- Conteúdos relacionados com o elemento ```<aside>```

No elemento ```<aside>``` utilizado quando buscamos destacar um trecho de um conteúdo ou artigo à parte (comerciais pagos, links promocionais), esse elemento também serve quando queremos chamar atenção para um dado adicional.
```html
  <aside>
    <h1>Tenha uma graduação</h1>
    <p>
      <a href="graduacao.com">
        Matricule-se já!
      <a/>
    </p>
  </aside> 
```

- Rodapé com o elemento ```<footer>```

O elemento ```<footer>``` representa o rodapé de um documento ou de uma seção específica do mesmo, podendo conter informações sobre direitos autorais, informações do autor, mídias sociais, política de privacidade, termos de serviço, entre outros.
``` html 
   <footer>
        <img src="logo.png">
        <p>Endereço: ...</p>
        <p>Telefone:(XX)XXXX-XXXX</p>
        <p>Todos os direitos reservados</p>
    </footer>
```

### Criando Listas

- Para criar uma lista *não ordenada* com marcadores

As listas não ordenadas são usadas para listar itens, sem se preocupar com sua sequência. Chamamos de lista de marcadores apenas.

Listas não ordenadas começam com um elemento `<ul>` de abertura, seguido por qualquer número de elementos `<li>`. Finalmente, as listas não ordenadas fecham com um `</ul>`
```html
<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>
```

- Para criar lista *ordenada* ou lista *numeradas*

As listas ordenadas ou numeradas são usadas para indicar alguma sequência ou numeração

Listas ordenadas começam com um elemento `<ol>` de abertura, seguido por qualquer número de elementos `<li>`. Finalmente, as listas ordenadas são fechadas com a tag `</ol>`.
```html
<ol>
  <li>Garfield</li>
  <li>Sylvester</li>
</ol>
```

### Adicionando imagens

Para adicionar imagens á página web é usado o elemento `img` e apontar para a URL de uma imagem especifica usando o atributo `src`.
```html
<img src="https://www.freecatphotoapp.com/your-image.jpg">
```

Todos os elementos img devem ter um atributo `alt`. O texto dentro de um atributo alt é usado para **leitores de tela para melhorar a acessibilidade** e é exibido se a imagem falhar ao carregar.
``` html
<img src="https://www.freecatphotoapp.com/your-image.jpg" alt="A business cat wearing a necktie.">
```

*Se a imagem for puramente decorativa, usar um atributo alt vazio é uma prática recomendada. Idealmente, o atributo alt não deve conter caracteres especiais, a menos que seja necessário.*

### Utilizando link

- Link para páginas externas

Para criar um link para conteúdo fora da página web pode-se usar o elemento `a` (ancora), que usa o atributo `href` que vai receber o link da página externa.
```html
<a href="https://www.freecodecamp.org">this links to freecodecamp.org</a>
```
- Link para páginas internas

O elemento `a` (ancora) também pode ser usado para criar links internos para diferentes seções em uma página da web.
Para criar um link interno é adicionado no link do atributo `href` o símbolo `#` mais o valor do atributo `id` para o elemento que será vinculado. É necessário adicionar o mesmo atributo `id` ao elemento ao qual está vinculando.
```html
<a href="#contacts-header">Contacts</a>
...
<h2 id="contacts-header">Contacts</h2>
```

Quando os usuários clicarem no link Contatos, eles são direcionados à seção da página da web com o elemento de cabeçalho Contatos.

- Aninhar um elemento âncora dentro de um parágrafo

É possível aninhar links em outros elementos de texto.
```html
<p>
  Here's a <a target="_blank" href="https://www.freecodecamp.org"> link to www.freecodecamp.org</a> for you to follow.
</p>
```

`target` é um atributo de marca de âncora que especifica **onde abrir o link**.

O valor `_blank` especifica para **abrir** o link em uma **nova guia**.

O `href`é um atributo de tag âncora que contém o endereço **URL do link**.

`top` abre o documento no corpo **todo da janela**.

- Link inativo

Para criar um link inativo, basta adicionar `#` no atributo `href`, ao invés da url.

É usado quando é necessaŕio adicionar elementos ao site antes de saber para onde eles serão vinculados.
```html
href="#"
```

- Transformar uma imagem em um link

É possível transformar elementos em links, aninhando-os em um elemento `a`.
```html
<a href="#">
	 <img src="https://www.bit.ly/fcc-running-cats" alt="Three kittens running towards the camera.">
</a>
```

*Depois de fazer isso, passe o cursor sobre a imagem. O ponteiro normal do cursor deve se tornar o ponteiro para clicar no link. A foto agora é um link.*

### Atributos de uma TAG

Atributos são informações que passamos na Tag para que ela se comporte da maneira esperada. Existem atributos globais (que funcionam em todas as Tags) e específicos (que são direcionados para cada Tag, através de especificação).

Os ***atributos*** possuem nome e um valor. Exemplo de atributo da tag <link>:
``` html
  <link rel="stylesheet" href="/assets/public/styles/css/style.css">
```
o atributo ```rel=""``` indica o valor da conexão, que no caso é ```rel="stylesheet"``` que significa "folha de estilo" para reconhecer o arquivo CSS externo. O atributo ```href=""``` significa o endereço dessa conexão, é importante que o endereço seja bem declarado para a conexão funcionar, senão não irá funcionar como esperado.

#### Atributos Específicos de uma TAG

| Atributo | Função do atributo |
| --- | --- |
| rel=" "	| Especifica o relacionamento entre o documento atual e o documento linkado |
| src=" "	| Especifica a URL do arquivo de mídia |
| type=" "	| Especifica o tipo do documento |
| alt=" "	| Mostra o texto quando a aparência não renderiza |
| target=" "	| Especifica o modo de abrir o link em janela |
| width=" "	| Especifica a largura do elemento |
| height=" "	| Especifica a altura do elemento |
| name=" "	| Especifica o nome do elemento |
| value=" "	| Especifica o valor do elemento |

#### Atributos Globais de uma TAG

| Atributo | Função do atributo |
| --- | --- |
| title=" "	| Especifica a informação extra sobre o elemento, como um balãosinho de texto |
| class=" "	| Especifica uma ou mais classes para um elemento ou varios elementos (referência de classe para o CSS) |
|id=" "	| Especifica uma unica id para um elemento (referência de id para o CSS) |

<hr>

<div align="center">
	<img alt="logo css na cor azul" src="https://welcometoalex.space/img/conhecimentos/css3.png" width="100">
</div>
	
CSS é abreviação de ***Cascading Style Sheet*** (folha de estilos em cascata). É a linguagem que define estilos para o HTML informando ao navegador como exibir os conteúdos, portanto, não se trata de linguagem de programação. CSS tem "cascata" no nome, devido a sua forma de determinar a propriedade de um elemento - levando em consideração hierarquia de seletores e de chamadas de estilo (inline, internal e external).
Com CSS é possível controlar a cor, fonte, tamanho, espaçamento entre outros aspectos dos elementos HTML.

<div align="center">
	<img alt="robo colorido ao lado bloco de codigo que altera a cor do robo" src="https://4.bp.blogspot.com/-tlvMaNOcvEI/VwDbHWHYVwI/AAAAAAAAOmA/vj17H7jxWYgunK8w0h-2P1IV_ynoMVYPQ/s1600/CSS%2Bminify%2Bof%2BBlogger%2BSpice.gif" width="350">
</div>
	
### Incluindo css na página

Existem três formas para incluir o código CSS em seu projeto:
	
- Estilo inline
	
 Neste método, o CSS é aplicado diretamente no elemento, utilizando o atributo ```style```. É caracterizado por possuir uma implementação mais simples, no entanto, este método dificulta a manutenção do código.
``` html
    <p style=?color: white; background:black?>Hello, world!</p>
```
	
- Estilo interno
	
 Caracteriza-se por escrever o código CSS, utilizando o comando ```<style>``` do HTML. Esse método é superior ao anterior, pois todas as regras CSS estão localizadas no ```<head>```. No entanto, essas regras só poderão ser utilizadas dentro deste documento, impedindo o compartilhamento e a reutilização das regras.
``` html
 <head>
  <style>
   * {margin: 0; padding: 0; box-sizing: border-box;}
   body {width: 100%; height: 100vh;}
  </style>
 </head>
```	
	
- Estilo externo
 Para fazer o link de um arquivo .css basta criar um ou mais arquivos com extensão .css e incluí-los na estrutura head do HTML, com o href do caminho do arquivo.
``` html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="css/style.css" />
  </head>
  <body></body>
</html>
```
	
Com o link também podemos importar fontes externas, exemplo [Google Fonts](https://fonts.google.com/)
``` html
<!DOCTYPE html>
<html>
  <head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Bona+Nova&display=swap" rel="stylesheet">
  </head>
  <body></body>
</html>
```
	
E no arquivo `.css` aplicar a regra
```
font-family: 'Bona Nova', serif;
```
	
### Seletores

Para escrever código CSS é necessário seguir uma regra. A regra é uma declaração que possui uma sintaxe própria bem simples que define a forma com que o estilo será aplicado aos nossos elementos HTML. 
	
- { propriedade: valor }

Dentro do arquivo `.css`, a sintaxe é:
``` html
seletor {
  propriedade: valor;
}
```
	
Exemplo:
``` hmtl
p {
  color: blue;
}
```
	
Explicando de forma grotesca o *seletor* nada mais é do que o nosso elemento HTML ao qual queremos aplicar a regra (por exemplo: div, body).

A *propriedade* é o atributo do elemento que será aplicado a regra. (por exemplo: color, font, position).

*Valor* é a característica que o elemento irá assumir (por exemplo: cor azul, tamanho 14 para a fonte).

*É uma boa prática terminar as declarações de estilo embutido com um ;*

- ID

É um seletor individual usado para vincular somente um elemento por página web. Ele não pode ser usado em dois ou mais elementos. Para construí-lo basta que você crie um nome precedido pelo símbolo #.
``` html
#nome-do-identificador {
   background-color: green; 
}
```
	
Veja agora com atribuir no HTML para que o elemento receba a cor de fundo verde:
``` html
<body id="nome-do-identificador">
</body>	
```

- Class

Este seletor possibilita o uso em mais de um elemento da mesma página. Indicado quando você precisa atribuir algumas propriedades iguais em elementos diferentes. Para construí-lo basta que você crie um nome precedido por um ponto.
``` html
	.nome-da-classe {
color: blue; 
}
```
	
Veja como atrbuir no elemento HTML
```html
<h1 class="nome-da-classe">Título com cor azul</h1>
```

### Principais Propriedades CSS

um resumo com as principais propriedades de estilo da linguagem CSS

- **font-family**: Define a família da fonte utilizada
```
font-family: Arial, Verdana, Geneva, sans-serif;
font-family: Arial, Verdana, Geneva, sans-serif;
```

- **font-style**: Define a propriedades de estilos que podem ser: normal, italic ou oblique.
```
font-style: italic;
font-style: normal;
```

- **font-weight** : Define a propriedade de intensidade de uma fonte na sequência de valores de ‘100’ a ‘900’, cada número indica uma fonte mais intensa (escura) que o valor anterior. 
```
font-weight: normal;  (ou valores de 100 a 500)
font-weight: bold;  (ou valores de 600 a 900)
```

- **font-size**: Define o tamanho da fonte. 
``` 
font-size: 12px;
```

- **letter-spacing**: Controla o espaçamento entre as letras de um texto.
``` 
letter-spacing: 5px;
```

- **word-spacing**: Controla o espaçamento entre as palavras de um texto.
``` 
word-spacing: 10px;
```

- **line-height**: Controla a altura entre as linhas do texto de um paragrafo.
``` 
line-height: 25px;
```

- **text-align**: Controla o posicionamento horizontal do conteúdo de um elemento. Os valores possíveis são: left, right, center e justify.
``` 
text-align: center;
```

- **text-decoration**: Define um efeito decorativo no texto. Podendo entre eles ser: none (sem decoração); underline (sublinhado); line-through(linha cortando o texto); e blink (efeito piscante).
``` 
text-decoration: underline;
```

- **text-transform**: Controla os efeitos de capitalização do texto. Com ela, podemos definir a caixa das letras (minúsculas e maiusculas). Os valores possíveis são:

 capitalize – transforma o primeiro caracter de cada palavra em maiúscula
 
 uppercase – transforma todas as letras de todas as palavras em maiúsculas
 
 lowercase – transforma todas as letras de todas as palavras em minúsculas
 
 none – cancela algum valor que tenha sido herdado
``` 
text-transform: uppercase;
```

- **text-indent**: Define o tamanho da endentação para a primeira linha do texto contida em um bloco, ou seja, o deslocamento para a direita de um paragrafo.
``` 
text-indent: 20px;
```

- **color**: Define a cor do texto de um texto.
``` 
color: red;

color: rgb(255,0,0);

color: #FF0000;
```

- **font**: Propriedade para definir em um único local vários estilos para a fonte. A sintaxe geral para font: [style] [variant] [weight] [size] [/line-height] [family].
``` 
font: normal small-caps bold 14px "Comic Sans MS", sans-serif;
```

> Os valores size e family são **obrigatórios**. Os demais são facultativos (se você os omitir será adotado o valor default ou herdado do elemento pai)

- **width**: Define o comprimento (largura) de um elemento.
```
width: 100px;
```

- **height**: Define a altura de um elemento.
 ```
height: 50px;
```

- **border**: Define bordas para um elemento.
 ```
border:1px solid #CCC;

border-bottom:5px solid #97B2B9;
```

- **background**: trata do fundo dos elementos. O elemento que mais recebe esta propriedade é o *body*.

	As propriedades do background são:
	
	- **color**: Define a cor do fundo.
	 ``` html
	div {
	  background-color: gray;
	}
	```

	- **image**: Define a imagem de fundo.

	*<b>url()</b>: Define a localização da imagem de fundo*.
	``` html
	div {
	  background-image: url("../img/bg.png");
	}
	```
	
	- **repeat**: Define a posição de repetição da imagem de fundo.

	*<b>no-repeat</b>: Não repete a imagem*.
	``` html
		div {
	  background-repeat: no-repeat;
	}
	```


- **opacity**: Especifica a opacidade/transparência de um elemento
A propriedade opacidade pode assumir um valor de **0,0 a 1,0**. Quanto menor o valor, mais transparente
```
img {
  opacity: 0.5;
}
```

- **margin**: Controla as margens de um elementos. Se forem indicados quatro valores, eles dizem respeito, respectivamente, às margens superior, direita, inferior e esquerda. Se for fornecido apenas um valor, ele é aplicado às quatro margens.
```
margin: 15px;

margin: 10px 1px 5px 20px;
```

A última atribuição so exemplo acima é:
```
margin-top: 10px;

margin-right: 1px;

margin-bottom: 5px;

margin-left: 20px;
```

- **padding**: Controla os espaçamentos de um elementos. Se forem indicados quatro valores, eles dizem respeito, respectivamente, aos espaçamentos superior, direito, inferior e esquerdo. Se for fornecido apenas um valor, ele é aplicado aos quatro espaçamentos.
```
padding: 5px;

padding: 10px 5px 5px 10px;
```

<div align="center">
	<img alt="homem arrumando cortina na janela" src="https://static.imasters.com.br/wp-content/uploads/2014/07/css-blinds.gif">
</div>

## É comum e super normal errar muitas vez o CSS, aprendê-lo requer práticar muitas vezes.
	
### Propriedade Display

Entender a propriedade display é fundamental para que possamos compreender o fluxo e estruturação de uma página web. Todos os elementos por padrão já possuem um valor para a propriedade e, geralmente estas são block ou inline.

> *Todo elemento em uma página web é renderizado como uma caixa retangular. A propriedade <b>display</b> de CSS vai determinar como essa caixa vai ser comportar*

#### Os possíveis tipos

- Block

O elemento se comporta como um **bloco**. Ocupando praticamente toda a largura disponível na página. Elementos de parágrafo (**p**) e título(**h1**, **h2**, ...) possuem esse comportamento por padrão.

- Inline

O elemento se comporta como um elemento em **linha**. Exemplos de elemento que se comportam assim são por exemplo as tags **span** e **a**.

- None

Ao contrários dos valores atuais, o valor none permite, informalmente dizendo, que você **desative** a propriedade do elemento. Quando você utiliza essa propriedade, o elemento e todos seus elementos filhos ***não são renderizados na página***.

Uma coisa importante a ressaltar que a propriedade **display: none** não é a mesma coisa da propriedade **visibility: hidden**. Nessa última o elemento não aparece na tela mas é renderizado na página, ou seja, vemos um espaço vazio no lugar do elemento; já a propriedade **display: none** não renderiza o elemento e, o espaço que era ocupado por ele, é ocupado pelo elemento seguinte no fluxo do documento.

- Table

O elemento se comporta como uma **tabela**.

- Inline-block

Semelhante ao inline, no entanto, ao definirmos **inline-block** em um elemento, conseguimos definir as propriedades de **largura** e **altura** para ele. Coisa que não conseguimos em um elemento com **display: inline**.

- Flex

É utilizado para organizar os elementos HTML de forma [responsiva](https://blog.betrybe.com/tecnologia/responsividade/). Na prática, ao definirmos um elemento com esse valor, ele funciona como um container para agrupar os elementos filhos, que são considerados flex-itens e são organizados nos sentidos horizontal ou vertical.


## Dicas extras (:

- Lorem Ipsum

A expressão [lorem ipsum](https://pt.wikipedia.org/wiki/Lorem_ipsum) é um texto padrão em latim utilizado por desenvolvedores web, designers gráficos, para preencher os espaços de texto em publicações (jornais, revistas, sites) para testar e ajustar aspectos visuais (layout, tipografia, formatação) antes de utilizar conteúdo real.

Alguns links criativos para gerar o lorem ipsum:

[catipsum](http://www.catipsum.com/);

[cupcakeipsum](http://www.cupcakeipsum.com/);

[pokemipsum](https://pokemipsum.com/);

[cheeseipsum](http://www.cheeseipsum.co.uk/);

- Cores 

[Nomes de Cores HTML&CSS](https://htmlcolorcodes.com/color-names/);

[Coolors - paleta de cores](https://coolors.co/);

[Flat UI Colors - paleta de cores](https://flatuicolors.com/);

- Extensão para selecionar cores

[ColorPick Eyedropper](https://chrome.google.com/webstore/detail/colorpick-eyedropper/ohcpnigalekghcmgcdcenkpelffpdolg);

[Color by Fardos](https://chrome.google.com/webstore/detail/color-by-fardos/iibpgpkhpfggipbacjfeijkloidhmiei);

[ColorPicker](https://chrome.google.com/webstore/detail/color-picker/mggikgocakmeahcgffajljnpnbcoaddn?hl=pt);

[CollorZilla](https://chrome.google.com/webstore/detail/colorzilla/bhlhnicpbhignbdhedgjhgdocnmhomnp?hl=pt);

- Fontes

[Google Fonts](https://fonts.google.com/);

[Extensão para visualizar fontes usadas pelo site](https://chrome.google.com/webstore/detail/fonts-ninja/eljapbgkmlngdpckoiiibecpemleclhh);

- Icones

[FlatIcon](https://www.flaticon.com/)

[FontAwesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2);

- Banco de Imagens

[Unsplash](https://unsplash.com/);

[Imagens de fundo](https://imagens-de-fundo.blogspot.com/);

[Freepik](https://br.freepik.com/);

[Imagens de pessoas negras e marrons](https://nappy.co/);

[Canva](https://www.canva.com/);

[Pixabay](https://pixabay.com/);

[Negativespace](https://negativespace.co/);

[Pexels](https://www.pexels.com/pt-br/);


<h4 align="center">Bons estudos !!!<h4>

<div align="center">
	<img alt="gato preto digitando no notebook" src="https://pa1.narvii.com/7317/bbcf367e85ac4467ed8a27be5870baf932a05552r1-480-480_hq.gif" width="280">
<div>
