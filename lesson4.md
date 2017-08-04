Tipografia
=========================

Títulos
-----------------------

```css
.h[1-6] {
    font-weight: 600; /* Semi Bold */
    font-size: 36px, 24px, 18px 14px e 12px;
}
```


Classes de título alternativo
-------------------------------

Útil para quando quiser aplicar estilo de um título, como espaçamento, a algum elemento, mas não quer usar a tag de títulos para, por exemplo, não interferir na estrutura semântica

```html
<div class="h1">
    <p>Este parágrafo será formatado com o mesmo estilo que um lemento H1, por causa da DIv que o contém</p>
</div>
```

Parágrafos
--------------------

É aplicado para `body` e qualquer elemento `P` dentro dele

```css
p {
    font-size: 14px;
    line-height: 1.428px;
}
```

Parágrafos Principais (Lead Paragraphs)
----------------------

```html
<!-- Obs.: Apenas representativo, aqui não aparecerá a formatação, pois não há como incluir classes CSS -->
<p>
    Este é um parágrafo normal com algumas sentenças. Nós trataremos este primeiro parágrafo como principal.
</p>
<p>
    Agora vamos voltar ao texto regular. Sem principal.
</p>
```

```css
.lead {
    font-size: 21px;
    font-weight: 300; /* Um pouco mais pesado que o normal */
}
```

Texto Tachado e Texto Deletado
------------------------------------

* A tag `S` representa semanticamente o tachado
* A tag `DEL`, apesar da mesma aparência, representa semanticamente, texto que foi deletado devido a uma edição ou revisão.

```html
<p><S>Este é texto tachado usando a tag S.</S></p>
<p><DEL>Este é texto deletado usando a tag DEL.</DEL></p>
```

Texto Sublinhado e Texto Inserido
-------------------------------------

Igual ao caso anterior, ambos exibem o mesmo estilo, mas possuem significado semantico diferente, use de acordo.

```html
<p><U>Este é um texto sublinhado</U></p>
<p><INS>Este é um texto inserido</INS></p>
```

Usar de acordo com o significado dá mais flexibilidade e permite a diferenciação, permitindo o uso de processos ou script para alterar o estilo.

Texto Destacado e Texto Pequeno
------------------------------------

* Small exibe o texto 85% de seu tipico tamanho por Bootstrap

```html
<p><MARK>Este texto está marcado com um efeito highlighter-style.</MARK></p>
<p>A próxima sentença está usando a tag small<SMALL>Este texto é menor do que o estilo o contendo</SMALL>Veja a comparação</p>
<h1>É mais fácil ver neste tamanho.<SMALL>Viu a diferença?</SMALL></h1>
```

Negrito e Itálico
-----------------------------------

* Vale a pena notar que negrito não atribui de verdade o font-weight com a palavra bold. É atribuido manualmente 700, isto mantém o weight mais padronizado através de diferentes navegadores. Alguns navegadores podem renderizar ligeiramente diferente.

```html
<STRONG>Nada terrivelmente incomum com texto em negritos</STRONG>
<EM>Mesma coisa com itálicos. eles parecem muito o mesmo.</EM>
```

Alinhamento de Texto e Justificação
-------------------------------------

```html
<p class="text-left">Este parágrafo está alinhado a esquerda.</p>
<p class="text-center">Este parágrafo está centralizado a seu container.</p>
<p class="text-right">Este parágrafo está alinhado a direita.</p>
<p class="text-justify">Este texto está justificado.</p>
```

Tranformação de texto
-------------------------------

```html
<p class="text-lowercase">ISTO FOI DIGITADO EM CAIXA ALTA.</p>
<p class="text-uppercase">isto foi digitado em caixa baixa.</p>
<p class="text-capitalize">Isto Foi Digitado Com A Primeira Em Maiuscula.</p>
```

Abreviações
---------------------------------

Por padrão o ABBR tem uma borda pontilhada e o cursor vira um ponto de interrogação de ajuda, adicionando a classe initialism a fonte reduz em 90%

```html
<p>O Estado de <ABBR title="Minas Gerais">MG</ABBR></p>

<p><ABBR class="initialism" title="Sociedade Brasileira de Computação">SBC</ABBR></p>
```

Address
-----------------------------------

Esta tag adiciona uma margem levemente mais larga na base de seu container.

```html
<ADDRESS>

    <STRONG>The Munsters</STRONG> <br>
    1313 Mockinbird Lane <br>
    Mockinbird Heights, CA, 91501
</ADDRESS>

<p>O próximo parágrafo ....</p>

```

Blockquotes
----------------------------------------

Adiciona uma linha lateral esquerda cinza e tamanho de fonte de 17.5px

* A classe `blockquote-reverse` alinha para a direita, inclusive a barra lateral

```html
<BLOCKQUOTE>
    <!-- Os matenedores do Bootstrap recomendam adicionar o elemento P no blockquote para a citação -->
    <P>Uma citação qualquer</P>
    <!-- Para adicionar uma fonte use o footer, o texto será 80% do tamanho padrão com uma cor cinza escura -->
    <FOOTER>Autor</FOOTER>
</BLOCKQUOTE>

```

Listas
--------------------------------------------

* A classe `list-unstyled` remove os marcadores e a margin esquerda

* A classe `list-inline` exibe os itens horizontalmente, em linha.

```html
<ol class="list-unstyled">
    <li>1</li>
    <li>2</li>
    <li>3</li>
</ol>

```

Listas de definição
-------------------------------------

* font-weight é setado com 700
* Use a classe `dl-horizontal` para exibir horizontalmente


```html
<DL class="dl-horizontal">
    <DT>Isto é um termo</DT>
    <DD>Isto é uma definição</DD>

    <DT>Isto é um termo</DT>
    <DD>Isto é uma definição</DD>

    <DT>Isto é um termo</DT>
    <DD>Isto é uma definição</DD>

</DL>

```

Documentação técnica
-----------------------------------

```html
<!-- fonte monoespaçada e uma caixa mais clara -->
<p><code><a href="#">Go learn!</a></code></p>
<!-- usado para exibir a entrada do usuário, usa uma fonte monoespaçada e uma caixa preta. Sugere que o usuário relamente precisa digitar estes comandos em seu próprio teclado  -->
<p><kbd>Aqui está o texto que você gostaria que o usuário introduzisse.</kbd></p>
<!-- Exibe multiplas linhas, com fonte espaçada e uma caixa -->
<p><pre>Esta é a tag PRE HTMl padrão</pre></p>
usada para exibir um pedaço de código
<p><samp>Este é um exemplo de saída de um hipotético programa</samp></p>

```
