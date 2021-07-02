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

### Essas são as linguagens client-side:

<div>
  <img alt="imagem do deadpool caveira, com cores e se mexendo" src="https://moz-static.moz.com/youmoz_uploads/javascript-seo/5948abfc0e2df5.02876591.gif" width="500">
</div>

Onde o HTML é responsavél pela <b>estrutura</b> da página, o CSS pela <b>estilização</b> e o JavaScript pela <b>interação</b>.

Nessas duas primeiras semanas iremos focar em <b>HTML & CSS</b>. 

## HTML
<div align="center">
  <img alt="logo hmtl na cor laranja" src="https://logodownload.org/wp-content/uploads/2016/10/html5-logo-8.png" width="100">
</div>
  
  HTML é abreviação de <b>Hyper Text Markup Language</b> é uma linguagem de marcação que usa uma sintaxe especial para descrever a estrutura de uma página da web para o navegador. Ou seja, não é uma linguagem de programação, pois não tem lógica (algoritmos).
  
- Tag

A maiora dos elementos HTML possui uma tag de abertura e uma tag de fechamento.
As tags de **abertura** têm a seguinte aparência:
``` html
<h1>
```
As tags de **fechamento** têm a seguinte aparência:
``` html
</h1>
```

- Títulos

Os elementos **h1** são frequentemente usados para **títulos principais**, enquanto os elementos **h2** são geralmente usados para **subtítulos**. Existem também elementos h3, h4, h5 e h6 para indicar diferentes níveis de subposições.

- Parágrafo

Os elementos **p** são os elementos usados para **texto de parágrafo** em sites. p é a abreviatura de "parágrafo".
``` html 
<p> Sou uma tag p! </p>
```

Por convenção, todas as tags HTML são escritas em minúsculas, por exemplo:
``` html
 <p> </p> 
```
e não 
``` html
<P> </P>
```

- Lorem Ipsum

A expressão [lorem ipsum](https://pt.wikipedia.org/wiki/Lorem_ipsum) é um texto padrão em latim utilizado por desenvolvedores web, designers gráficos, para preencher os espaços de texto em publicações (jornais, revistas, sites) para testar e ajustar aspectos visuais (layout, tipografia, formatação) antes de utilizar conteúdo real.

Alguns links criativos para gerar o lorem ipsum:

[catipsum](http://www.catipsum.com/)

[cupcakeipsum](http://www.cupcakeipsum.com/)

[pokemipsum](https://pokemipsum.com/)

[cheeseipsum](http://www.cheeseipsum.co.uk/)

- Comentários

``` html
<!-- Isso é um comentário. Comentar é uma maneira de deixar comentários para outros desenvolvedores em meu código, sem afetar a saída resultante que é exibida para o usuário final.
Os comentários também são uma maneira conveniente de tornar o código inativo sem ter que excluí-lo por completo.-->
```
