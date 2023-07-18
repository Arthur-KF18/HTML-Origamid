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
