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

<img src="https://sites.google.com/site/uniplibancodedados1/aulas/aula-7---tipos-de-relacionamento/aula_7_relacionamento.bmp?attredirects=0">
