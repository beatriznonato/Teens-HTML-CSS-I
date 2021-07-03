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

<hr>
<div align="center">
  <img alt="logo hmtl na cor laranja" src="https://logodownload.org/wp-content/uploads/2016/10/html5-logo-8.png" width="100">
</div>

## HTML
  HTML é abreviação de <b>Hyper Text Markup Language</b> é uma linguagem de marcação que usa uma sintaxe especial para descrever a estrutura de uma página da web para o navegador. Ou seja, não é uma linguagem de programação, pois não tem lógica (algoritmos).
  
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



