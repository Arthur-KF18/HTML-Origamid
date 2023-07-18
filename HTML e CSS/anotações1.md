# HTML e CSS básico

- Anotações da segunda aula de HTML da Origamid

#### Link Caminhos

- Existem dois tipos de caminhos __dentro do HTML que vão direcionar para outras páginas__:
  - Absoluto: `<a href="https://www.origamid.com/cursos/">Origamid Cursos</a>`
  - Relativo: `<a href="/produtos/bicicletas.html">Bicicletas</a>`
    - A __principal diferença entre ambos os caminhos, é de que o absoluto leva para uma outra página na web já existente, enquanto no relativo, ela irá levar a outra página presente apenas no documento atual__
- Além disto, temos diferentes formas de acessar os arquivos no mesmo documento, __são chamados de Caminho Relativo__:
  - `/index.html`: Arquivo `index.html` no diretório raiz `/`
  - `/produtos/bicicletas.html`: Arquivo `bicicletas.html` no diretório `/produtos` localizado na raiz
  - `index.html` ou `./index.html`: Arquivo `index.html` no diretório atual `./`
  - `../index.html`: Arquivo `index.html` um diretório anterior ao atual `../`
  - `../../index.html`: Arquivo `index.html` dois diretórios anteriores ao atual
- No nosso código, se escrevermos assim:

```htm
<h1>Carros e Bicicletas</h1>
    <a href="produtos/carros.html">Carros</a>
    <a href="produtos/bicicletas.html">Bicicletas</a>
```

- O que ocorre é que __quando mandamos ele procurar a pasta produtos, será no diretório atual e nele ocorrerá a busca, trazendo os arquivos de páginas que solicitamos__

#### CSS Básico

- __Sempre colocamos nas tags `<head>` do nosso documento html__
- link: Cria uma relação entre um documento HTML e um arquivo de estilo CSS.
- rel : Define o tipo de arquivo (stylesheet para CSS). __É possível linkar outros também como favicons.__
- O css funciona da seguinte maneira:

```css
a {
  color: black;
  text-decoration: none;
}
```

- a: Seletor que estamos querendo
- {} : bloco do css
- `color` ou `text-decoration`: propriedade que escrevemos
- `black`: valor da propriedade, sendo qualquer que esteja sendo aplicada
- em resumo:

```css
seletor {
  propriedade: valor;
}
```

- A __ordem dos elementos dentro dos arquivos CSS e do HTML irá definir o estilo selecionado__

#### CSS Seletores

- h1, p: A vírgula permite selecionarmos múltiplos elementos para a aplicação de um mesmo estilo.
- p a: Seleciona o `a` que tiver um `p` como elemento pai (não precisa ser filho direto).
- Por exemplo, se aplicarmos:

```css
  html a {
    color: wheat;
  }
```

- Será aplicada a cor especificada __a todo documento, e que será a todos os `a` presentes__
- __Um fator importante sobre os seletores de id, que acompanham `id=""`, além de serem personalizados no css com o seletor `#nomedoid`, ele é muito específico. O problema entre ele e a as classes, é de que geralmente o id é atrelado ao JavaScript. Se termos uma função no js que procure um id específico, a repetição dele no nosso código quebraria a página__
- Podemos adicionar mais de uma classe em uma tag HTML:

```html
<h2 class="azul grande underline">Curso de Programação</h2>
```

#### HTML Exercício

1 - Crie um projeto chamado cinema.

2 - Crie um arquivo index.html
2.1 - O título do arquivo e o título de nível 1 devem conter o nome do projeto.

3 - Crie um diretório dentro do projeto com nome de: estados

4 - Em estados crie dois arquivos: rj.html e sp.html
4.1 - Adicionar link levando para o início do site.
4.2 - Adicionar título de nível 1 com o nome do estado.
4.3 - Adicionar os seguintes parágrafos (cada filme é um parágrafo):

(Rio de Janeiro)
Lisbela e o Prisioneiro - 20:00 - Hoje
Meu nome não é Jhonny - 21:00 - Hoje
O Cheiro do ralo - 15:00 - Amanhã

(São Paulo)
Lisbela e o Prisioneiro - 20:00 - Hoje
Meu nome não é Jhonny - 21:00 - Amanhã
O Cheiro do ralo - 15:00 - Amanhã

5 - Crie um link para cada cidade na página inicial para.
5.1 - O link deve estar dentro de um título de nível 2.

6 - Crie um arquivo de estilo dentro de um diretório chamado css.
6.1 - Link o arquivo em todas as páginas.
6.2 - Mude a cor dos filmes que estreiam hoje para darkred.
6.3 - Mude a cor dos filmes que estreiam amanhã para darkblue.
6.4 - Remova o sublinhado de todos os links do site.
6.5 - Mude a cor dos links que estão dentro do título de nível 2 para seagreen.
6.6 - Aumente a fonte dos parágrafos para 20px.
6.7 - Mude a família da fonte de todo o site para Arial.