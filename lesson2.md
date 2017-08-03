Grid do Bootstrap
===============

* 12 colunas de largura

* 4 breakpoints para diferentes larguras de tela
    + Menor do que 768px é **extra small** (Pense nos telefones)
    + Entre 768px e 991px é **small** (Pense nos tablets)
    + Entre 992px e 1199px é **medium** (Pense em laptops de tela pequena e desktops)
    + Maior que 1200px é **large**

* O breakpoint mais baixo aplicável se aplica

* Se nenhum breakpoint é especificado, a coluna empilha verticalmente

Linhas e Colunas do Bootstrap
-----------------------------

* Usa linguagem similar a tabelas, porém não usa a tag TABLE

* Muito mais fácil do que tabelas HTML, sendo compatível com os padrões e soar semanticamente


Podemos adicionar uma calha (gutter) entre as colunas adicionando padding

Qualquer estilo aplicado a um breakpoint, é aplicado automaticamente para os breakpoints mais largos a menos que você explicitamente provenha estilos para os breakpoints mais largos

Tamanhos das colunas do Bootstrap

|                   | Extra Small | Small     | Medium    | Large      |
| :-------------    | :---------- | :-------- | :-------- | :--------- |
| Breakpoint        | < 768px     | >= 768px  | 970px     | >= 1200px  |
| Largura da coluna | Automático  | 62px      | 81px      | 97px       |
| Largura da calha  |             30px - 15px em cada lado
