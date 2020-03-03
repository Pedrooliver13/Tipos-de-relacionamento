<h2><strong>TIPOS DE RELACIONAMENTO</strong></h2>

<p>De acordo com a cardinalidade existem 3 tipos básicos de relacionamentos entre as entidades.</p>


RELACIONAMENTOS UM PARA MUITOS<br>
RELACIONAMENTOS MUITOS PARA MUITOS<br>
RELACIONAMENTOS UM PARA MUITOS<br>


<h2>RELACIONAMENTO UM PARA MUITOS (U:M)</h2>

<p>
  Um relacionamento 1:m ocorre com freqüência em situações de negócio. Às vezes ocorre em forma de árvore ou em forma hierárquica. 
  No exemplo abaixo, temos a seguinte representação: Cada curso cadastrado possui vários alunos ligados a ele, pois cada aluno, ao ser cadastrado, 
  deverá ser ligado a um curso obrigatóriamente. O campo codigocurso foi escolhido como chave primária na entidade CURSO, ou seja, ela não poderá se repetir. Já na tabela ALUNO, a chave primária é matricula e o codigocurso é chave estrangeira. A representação ficaria assim
</p>

<img align="center" src="https://sites.google.com/site/uniplibancodedados1/aulas/aula-7---tipos-de-relacionamento/aula_7_relacionamento.bmp?attredirects=0" alt="1:1">

Como lemos este relacionamento:<br>

UM CURSO MATRICULA MUITOS ALUNOS<br>
UM ALUNO SE MATRICULA EM UM CURSO<br>

<h2>RELACIONAMENTOS MUITOS PARA MUITOS (M:M)</h2>

<p>Uma ocorrencia de uma entidade em A está associada a qualquer número de ocorrencias na entidade B, e cada ocorrencia da entidade em B está associada a qualquer número de ocorrencias na entidade A.</p>

<p>
  Considere o caso em que itens são vendidos. Podemos identificar imediatamente duas entidades: VENDA e ITEM. Uma venda pode consistir em muitos itens de mercadorias e um item de mercadoria pode aparecer em muitas vendas. Não estamos dizendo que um mesmo item possa ser vendido muitas vezes, mas que o tipo específico de item (por exemplo, um livro ) pode ser vendido muitas vezes; temos, portanto, um relacionamento de muitos-para-muitos (m:m) entre VENDA e ITEM. Em um relacionamento m:m, criamos uma terceira entidade, chamada entidade associativa que é usada para associar as entidades por meio de dois relacionamentos 1:m. De maneira geral, é razoavelmente fácil nomear essa terceira entidade. Nesse exemplo, essa terceira entidade, geralmente conhecida como entidade associativa, é chamada de VENDA_MERCADORIA.
</p>

<p>Observe a ficha abaixo. Observe a representação do relacionamento. Cada uma das linhas que aparece no formulário do pedido de vendas é, em geral, conhecida no varejo como um item de linha, onde o código da mercadoria é ligado a uma venda.</p>

<img align="center" src="https://sites.google.com/site/uniplibancodedados1/aulas/aula-7---tipos-de-relacionamento/aula_7_relacionamento2.bmp?attredirects=0">

<p>
A representação desse relacionamento m:m é mostrada na figura acima. Dizemos muitos para muitos porque há dois relacionamentos: CODIGO DA MERCADORIA está relacionado com muitas VENDAS e VENDA está relacionada com muitos CÓDIGOS DE MERCADORIA.
</p>

<p>
  No caso do nosso exemplo, a entidade associativa é a VENDA_MERCADORIA. Podemos fazer a leitura do relacionamento acima da seguinte forma:
</p>

