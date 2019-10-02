"# PHP-Aula07-ex9" 
<?xml version="1.0" encoding="utf-8"?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" lang="en" xml:lang="en">
<head>
<!-- 2019-10-01 ter 21:47 -->
<meta http-equiv="Content-Type" content="text/html;charset=utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>&lrm;</title>
<meta name="generator" content="Org mode" />
<style type="text/css">
 <!--/*--><![CDATA[/*><!--*/
  .title  { text-align: center;
             margin-bottom: .2em; }
  .subtitle { text-align: center;
              font-size: medium;
              font-weight: bold;
              margin-top:0; }
  .todo   { font-family: monospace; color: red; }
  .done   { font-family: monospace; color: green; }
  .priority { font-family: monospace; color: orange; }
  .tag    { background-color: #eee; font-family: monospace;
            padding: 2px; font-size: 80%; font-weight: normal; }
  .timestamp { color: #bebebe; }
  .timestamp-kwd { color: #5f9ea0; }
  .org-right  { margin-left: auto; margin-right: 0px;  text-align: right; }
  .org-left   { margin-left: 0px;  margin-right: auto; text-align: left; }
  .org-center { margin-left: auto; margin-right: auto; text-align: center; }
  .underline { text-decoration: underline; }
  #postamble p, #preamble p { font-size: 90%; margin: .2em; }
  p.verse { margin-left: 3%; }
  pre {
    border: 1px solid #ccc;
    box-shadow: 3px 3px 3px #eee;
    padding: 8pt;
    font-family: monospace;
    overflow: auto;
    margin: 1.2em;
  }
  pre.src {
    position: relative;
    overflow: visible;
    padding-top: 1.2em;
  }
  pre.src:before {
    display: none;
    position: absolute;
    background-color: white;
    top: -10px;
    right: 10px;
    padding: 3px;
    border: 1px solid black;
  }
  pre.src:hover:before { display: inline;}
  /* Languages per Org manual */
  pre.src-asymptote:before { content: 'Asymptote'; }
  pre.src-awk:before { content: 'Awk'; }
  pre.src-C:before { content: 'C'; }
  /* pre.src-C++ doesn't work in CSS */
  pre.src-clojure:before { content: 'Clojure'; }
  pre.src-css:before { content: 'CSS'; }
  pre.src-D:before { content: 'D'; }
  pre.src-ditaa:before { content: 'ditaa'; }
  pre.src-dot:before { content: 'Graphviz'; }
  pre.src-calc:before { content: 'Emacs Calc'; }
  pre.src-emacs-lisp:before { content: 'Emacs Lisp'; }
  pre.src-fortran:before { content: 'Fortran'; }
  pre.src-gnuplot:before { content: 'gnuplot'; }
  pre.src-haskell:before { content: 'Haskell'; }
  pre.src-hledger:before { content: 'hledger'; }
  pre.src-java:before { content: 'Java'; }
  pre.src-js:before { content: 'Javascript'; }
  pre.src-latex:before { content: 'LaTeX'; }
  pre.src-ledger:before { content: 'Ledger'; }
  pre.src-lisp:before { content: 'Lisp'; }
  pre.src-lilypond:before { content: 'Lilypond'; }
  pre.src-lua:before { content: 'Lua'; }
  pre.src-matlab:before { content: 'MATLAB'; }
  pre.src-mscgen:before { content: 'Mscgen'; }
  pre.src-ocaml:before { content: 'Objective Caml'; }
  pre.src-octave:before { content: 'Octave'; }
  pre.src-org:before { content: 'Org mode'; }
  pre.src-oz:before { content: 'OZ'; }
  pre.src-plantuml:before { content: 'Plantuml'; }
  pre.src-processing:before { content: 'Processing.js'; }
  pre.src-python:before { content: 'Python'; }
  pre.src-R:before { content: 'R'; }
  pre.src-ruby:before { content: 'Ruby'; }
  pre.src-sass:before { content: 'Sass'; }
  pre.src-scheme:before { content: 'Scheme'; }
  pre.src-screen:before { content: 'Gnu Screen'; }
  pre.src-sed:before { content: 'Sed'; }
  pre.src-sh:before { content: 'shell'; }
  pre.src-sql:before { content: 'SQL'; }
  pre.src-sqlite:before { content: 'SQLite'; }
  /* additional languages in org.el's org-babel-load-languages alist */
  pre.src-forth:before { content: 'Forth'; }
  pre.src-io:before { content: 'IO'; }
  pre.src-J:before { content: 'J'; }
  pre.src-makefile:before { content: 'Makefile'; }
  pre.src-maxima:before { content: 'Maxima'; }
  pre.src-perl:before { content: 'Perl'; }
  pre.src-picolisp:before { content: 'Pico Lisp'; }
  pre.src-scala:before { content: 'Scala'; }
  pre.src-shell:before { content: 'Shell Script'; }
  pre.src-ebnf2ps:before { content: 'ebfn2ps'; }
  /* additional language identifiers per "defun org-babel-execute"
       in ob-*.el */
  pre.src-cpp:before  { content: 'C++'; }
  pre.src-abc:before  { content: 'ABC'; }
  pre.src-coq:before  { content: 'Coq'; }
  pre.src-groovy:before  { content: 'Groovy'; }
  /* additional language identifiers from org-babel-shell-names in
     ob-shell.el: ob-shell is the only babel language using a lambda to put
     the execution function name together. */
  pre.src-bash:before  { content: 'bash'; }
  pre.src-csh:before  { content: 'csh'; }
  pre.src-ash:before  { content: 'ash'; }
  pre.src-dash:before  { content: 'dash'; }
  pre.src-ksh:before  { content: 'ksh'; }
  pre.src-mksh:before  { content: 'mksh'; }
  pre.src-posh:before  { content: 'posh'; }
  /* Additional Emacs modes also supported by the LaTeX listings package */
  pre.src-ada:before { content: 'Ada'; }
  pre.src-asm:before { content: 'Assembler'; }
  pre.src-caml:before { content: 'Caml'; }
  pre.src-delphi:before { content: 'Delphi'; }
  pre.src-html:before { content: 'HTML'; }
  pre.src-idl:before { content: 'IDL'; }
  pre.src-mercury:before { content: 'Mercury'; }
  pre.src-metapost:before { content: 'MetaPost'; }
  pre.src-modula-2:before { content: 'Modula-2'; }
  pre.src-pascal:before { content: 'Pascal'; }
  pre.src-ps:before { content: 'PostScript'; }
  pre.src-prolog:before { content: 'Prolog'; }
  pre.src-simula:before { content: 'Simula'; }
  pre.src-tcl:before { content: 'tcl'; }
  pre.src-tex:before { content: 'TeX'; }
  pre.src-plain-tex:before { content: 'Plain TeX'; }
  pre.src-verilog:before { content: 'Verilog'; }
  pre.src-vhdl:before { content: 'VHDL'; }
  pre.src-xml:before { content: 'XML'; }
  pre.src-nxml:before { content: 'XML'; }
  /* add a generic configuration mode; LaTeX export needs an additional
     (add-to-list 'org-latex-listings-langs '(conf " ")) in .emacs */
  pre.src-conf:before { content: 'Configuration File'; }

  table { border-collapse:collapse; }
  caption.t-above { caption-side: top; }
  caption.t-bottom { caption-side: bottom; }
  td, th { vertical-align:top;  }
  th.org-right  { text-align: center;  }
  th.org-left   { text-align: center;   }
  th.org-center { text-align: center; }
  td.org-right  { text-align: right;  }
  td.org-left   { text-align: left;   }
  td.org-center { text-align: center; }
  dt { font-weight: bold; }
  .footpara { display: inline; }
  .footdef  { margin-bottom: 1em; }
  .figure { padding: 1em; }
  .figure p { text-align: center; }
  .inlinetask {
    padding: 10px;
    border: 2px solid gray;
    margin: 10px;
    background: #ffffcc;
  }
  #org-div-home-and-up
   { text-align: right; font-size: 70%; white-space: nowrap; }
  textarea { overflow-x: auto; }
  .linenr { font-size: smaller }
  .code-highlighted { background-color: #ffff00; }
  .org-info-js_info-navigation { border-style: none; }
  #org-info-js_console-label
    { font-size: 10px; font-weight: bold; white-space: nowrap; }
  .org-info-js_search-highlight
    { background-color: #ffff00; color: #000000; font-weight: bold; }
  .org-svg { width: 90%; }
  /*]]>*/-->
</style>
<script type="text/javascript">
/*
@licstart  The following is the entire license notice for the
JavaScript code in this tag.

Copyright (C) 2012-2019 Free Software Foundation, Inc.

The JavaScript code in this tag is free software: you can
redistribute it and/or modify it under the terms of the GNU
General Public License (GNU GPL) as published by the Free Software
Foundation, either version 3 of the License, or (at your option)
any later version.  The code is distributed WITHOUT ANY WARRANTY;
without even the implied warranty of MERCHANTABILITY or FITNESS
FOR A PARTICULAR PURPOSE.  See the GNU GPL for more details.

As additional permission under GNU GPL version 3 section 7, you
may distribute non-source (e.g., minimized or compacted) forms of
that code without the copy of the GNU GPL normally required by
section 4, provided you include this license notice and a URL
through which recipients can access the Corresponding Source.


@licend  The above is the entire license notice
for the JavaScript code in this tag.
*/
<!--/*--><![CDATA[/*><!--*/
 function CodeHighlightOn(elem, id)
 {
   var target = document.getElementById(id);
   if(null != target) {
     elem.cacheClassElem = elem.className;
     elem.cacheClassTarget = target.className;
     target.className = "code-highlighted";
     elem.className   = "code-highlighted";
   }
 }
 function CodeHighlightOff(elem, id)
 {
   var target = document.getElementById(id);
   if(elem.cacheClassElem)
     elem.className = elem.cacheClassElem;
   if(elem.cacheClassTarget)
     target.className = elem.cacheClassTarget;
 }
/*]]>*///-->
</script>
</head>
<body>
<div id="content">
<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#org149c9b7">1. Classes</a>
<ul>
<li><a href="#orgc8533be">1.1. Definir uma classe</a></li>
<li><a href="#orgc0aae0e">1.2. Definindo objetos</a></li>
<li><a href="#org81594d1">1.3. Utilizando m�todos</a></li>
<li><a href="#org2124dec">1.4. Modificador de acesso</a></li>
<li><a href="#orgfddfdf0">1.5. Construtor</a></li>
</ul>
</li>
<li><a href="#org4e01ab4">2. Mysqli orientado a objetos</a>
<ul>
<li><a href="#orgdf1ce35">2.1. Abrindo a conex�o</a></li>
<li><a href="#orga9ed1ef">2.2. Fechar a conex�o</a></li>
<li><a href="#orgef43aa4">2.3. Exerc�cio 1</a></li>
<li><a href="#org512ee87">2.4. Criando banco de dados</a></li>
<li><a href="#orgedc2ea5">2.5. Exerc�cio 2</a></li>
<li><a href="#org79c21a2">2.6. Criando tabelas</a></li>
<li><a href="#org8eb62e0">2.7. Exerc�cio 3</a></li>
<li><a href="#orgc4d5ce6">2.8. Inserindo dados</a></li>
<li><a href="#orgfbe751c">2.9. Criptografia</a></li>
<li><a href="#orgaf2227c">2.10. Exerc�cio 4</a></li>
<li><a href="#org33908b5">2.11. Selecionando dados</a></li>
<li><a href="#org728feec">2.12. Exerc�cio 5</a></li>
<li><a href="#orgb09df94">2.13. Exerc�cio 6</a></li>
<li><a href="#orge93a97c">2.14. Exerc�cio 7</a></li>
<li><a href="#orgeb01153">2.15. Exerc�cio 8</a></li>
<li><a href="#orgd34fca4">2.16. Exerc�cio 9</a></li>
</ul>
</li>
</ul>
</div>
</div>

<div id="outline-container-org149c9b7" class="outline-2">
<h2 id="org149c9b7"><span class="section-number-2">1</span> Classes</h2>
<div class="outline-text-2" id="text-1">
</div>
<div id="outline-container-orgc8533be" class="outline-3">
<h3 id="orgc8533be"><span class="section-number-3">1.1</span> Definir uma classe</h3>
<div class="outline-text-3" id="text-1-1">
<p>
A palavra chave <b>class</b> define uma classe em PHP:
</p>

<pre class="example">
class Carro {
  // propriedades do carro

  // m�todos do carro
}
</pre>

<p>
Ajustamos as propriedades como vari�veis dentro da classe:
</p>

<pre class="example">
class Carro {
  $portas = 2;
  $cor = "black";
  $rodas = 14;

  // m�todos do carro
}
</pre>

<p>
M�todos s�o ajustados como fun��es dentro da classe.
</p>

<pre class="example">
class Carro {
  $portas = 2;
  $cor = "black";
  $rodas = 14;
  $velocidade = 0;

  function acelera() {
     $velocidade = $velocidade + 10;
  }

  function freia() {
     $velocidade = $velocidade - 10;
  }
}
</pre>
</div>
</div>

<div id="outline-container-orgc0aae0e" class="outline-3">
<h3 id="orgc0aae0e"><span class="section-number-3">1.2</span> Definindo objetos</h3>
<div class="outline-text-3" id="text-1-2">
<p>
Definidas as classes podemos criar objetos usando <b>new</b>:
</p>

<pre class="example">
class Carro {
  $portas = 2;
  $cor = "black";
  $rodas = 14;
  $velocidade = 0;

  function acelera() {
     $velocidade = $velocidade + 10;
  }

  function freia() {
     $velocidade = $velocidade - 10;
  }

  function get_velocidade() {
     return $velocidade;
  }
}

$fusca = new Carro();
$ferrari = new Carro();
</pre>
</div>
</div>

<div id="outline-container-org81594d1" class="outline-3">
<h3 id="org81594d1"><span class="section-number-3">1.3</span> Utilizando m�todos</h3>
<div class="outline-text-3" id="text-1-3">
<p>
Criados os objetos podemos utilizar os m�todos usando <b>-&gt;</b>:
</p>

<pre class="example">
$fusca = new Carro();
$ferrari = new Carro();

$fusca-&gt;acelera():
$fusca-&gt;acelera();

echo $fusca-&gt;get_velocidade();

$ferrari-&gt;acelera();

echo $ferrari-&gt;get_velocidade();
</pre>
</div>
</div>

<div id="outline-container-org2124dec" class="outline-3">
<h3 id="org2124dec"><span class="section-number-3">1.4</span> Modificador de acesso</h3>
<div class="outline-text-3" id="text-1-4">
<p>
Podemos modificar o tipo de acesso das propriedades da classe e dos m�todos:
</p>

<ul class="org-ul">
<li>public - a propriedade ou m�todo pode ser vista por qualquer um (padr�o).</li>
<li>protected - somente a pr�pria classe e derivadas podem acessar a propriedade ou m�todo.</li>
<li>private - somente a pr�pria classe pode acessar a propriedade ou m�todo.</li>
</ul>

<pre class="example">
class Carro {
  private $portas = 2;
  private $cor = "black";
  private $rodas = 14;
  public $velocidade = 0;

  function acelera() {
     $velocidade = $velocidade + 10;
  }

  function freia() {
     $velocidade = $velocidade - 10;
  }

  function get_velocidade() {
     return $velocidade;
  }
}

$ferrari = new Carro();

echo $ferrari-&gt;velocidade;
</pre>
</div>
</div>

<div id="outline-container-orgfddfdf0" class="outline-3">
<h3 id="orgfddfdf0"><span class="section-number-3">1.5</span> Construtor</h3>
<div class="outline-text-3" id="text-1-5">
<p>
A fun��o __construct permite inicializar uma propriedade de um objeto no momento da cria��o do objeto.
</p>

<p>
Se voc� criar uma fun��o <b>__construct()</b> o PHP vai execut�-la automaticamente quando voc� criar um objeto da classe.
</p>

<pre class="example">
class Carro {
  public $velocidade = 0;

  function acelera() {
     $velocidade = $velocidade + 10;
  }

  function freia() {
     $velocidade = $velocidade - 10;
  }

  function __construct() {
     $velocidade = 10;
  }
}

$ferrari = new Carro();

echo $ferrari-&gt;velocidade; // Come�a com 10
</pre>
</div>
</div>
</div>


<div id="outline-container-org4e01ab4" class="outline-2">
<h2 id="org4e01ab4"><span class="section-number-2">2</span> Mysqli orientado a objetos</h2>
<div class="outline-text-2" id="text-2">
</div>
<div id="outline-container-orgdf1ce35" class="outline-3">
<h3 id="orgdf1ce35"><span class="section-number-3">2.1</span> Abrindo a conex�o</h3>
<div class="outline-text-3" id="text-2-1">
<p>
Antes de acessar os dados em um banco de dados MySQL, voc� precisa se conectar ao servidor:
</p>

<pre class="example">
&lt;?php

$servidor = "localhost";
$usuario = "root";
$senha = "toor";

// Cria a conex�o:
// Novo objeto!
$conexao = new mysqli($servidor, $usuario, $senha);

// Verifica a conex�o
// Atributo do objeto $conexao
if( $conexao-&gt;connect_error ) {
   die("A conex�o falhou: " . $conexao-&gt;connect_error());
}

echo "Conex�o realizada com sucesso!";
?&gt;
</pre>
</div>
</div>


<div id="outline-container-orga9ed1ef" class="outline-3">
<h3 id="orga9ed1ef"><span class="section-number-3">2.2</span> Fechar a conex�o</h3>
<div class="outline-text-3" id="text-2-2">
<p>
Quando o script termina, a conex�o com o banco de dados � fechada automaticamente. Mas podemos fech�-la antes:
</p>

<pre class="example">
// m�todo do objeto $conexao
$conexao-&gt;close();
</pre>
</div>
</div>

<div id="outline-container-orgef43aa4" class="outline-3">
<h3 id="orgef43aa4"><span class="section-number-3">2.3</span> Exerc�cio 1</h3>
<div class="outline-text-3" id="text-2-3">
<p>
Crie uma p�gina php chamada (teste.php) que verifica se a conex�o com o servidor de banco de dados est� sendo feita corretamente utilizando mysqli orientado a objetos.
</p>
</div>
</div>

<div id="outline-container-org512ee87" class="outline-3">
<h3 id="org512ee87"><span class="section-number-3">2.4</span> Criando banco de dados</h3>
<div class="outline-text-3" id="text-2-4">
<p>
Para criar o banco em PHP voc� efetua uma consulta (query) com o comando de cria��o:
</p>

<pre class="example">
$sql = "CREATE DATABASE prova";

// executando um m�todo de $conexao
if ($conexao-&gt;query($sql) === TRUE) {
    echo "Banco de dados criado";
} else {
    // acessando a propriedade error de $conexao
    echo "Erro na cria��o do banco: " . $conexao-&gt;error; 
}
</pre>

<p>
A p�gina completa deve:
</p>

<ul class="org-ul">
<li>criar a conex�o com o servidor de banco de dados</li>
<li>efetuar a consulta</li>
<li>fechar a conex�o</li>
</ul>

<pre class="example">
&lt;?php

$servidor = "localhost";
$usuario = "root";
$senha = "toor";

// Cria a conex�o:
// Novo objeto!
$conexao = new mysqli($servidor, $usuario, $senha);

// Verifica a conex�o
// Atributo do objeto $conexao
if( $conexao-&gt;connect_error ) {
   die("A conex�o falhou: " . $conexao-&gt;connect_error());
}

echo "Conex�o realizada com sucesso!";

$sql = "CREATE DATABASE prova";

// executando um m�todo de $conexao
if ($conexao-&gt;query($sql) === TRUE) {
    echo "Banco de dados criado";
} else {
    // acessando a propriedade error de $conexao
    echo "Erro na cria��o do banco: " . $conexao-&gt;error; 
}

// m�todo do objeto $conexao
$conexao-&gt;close();
?&gt;
</pre>
</div>
</div>

<div id="outline-container-orgedc2ea5" class="outline-3">
<h3 id="orgedc2ea5"><span class="section-number-3">2.5</span> Exerc�cio 2</h3>
<div class="outline-text-3" id="text-2-5">
<p>
Criaremos um sistema de listas, o usu�rio far� um cadastro no sistema, efetuar� login, cadastrar� uma lista e criar� itens da lista. Portanto vamos precisar de um banco chamado <b>sistema</b>.
</p>

<p>
Escreva uma p�gina em php (cria.php) que cria um banco de dados chamado: <b>sistema</b>.
</p>
</div>
</div>

<div id="outline-container-org79c21a2" class="outline-3">
<h3 id="org79c21a2"><span class="section-number-3">2.6</span> Criando tabelas</h3>
<div class="outline-text-3" id="text-2-6">
<p>
O m�todo mysqli para executar um comando SQL � <b>query()</b> e deve ser executado em um objeto mysqli:
</p>

<pre class="example">
$conexao-&gt;query($sql)
</pre>

<p>
A p�gina completa orientada a objetos que cria uma tabela �:
</p>

<pre class="example">
&lt;?php
$servidor = "localhost";
$usuario = "root";
$senha = "toor";
$banco = "bdEscola"; // novo campo

// Cria a conex�o:
// Novo objeto!
$conexao = new mysqli($servidor, $usuario, $senha, $banco);

// Verifica a conex�o
// Atributo do objeto $conexao
if( $conexao-&gt;connect_error ) {
   die("A conex�o falhou: " . $conexao-&gt;connect_error());
}

echo "Conex�o realizada com sucesso!";

$sql = "CREATE TABLE alunos (
   id INT(6) UNSIGNED AUTO_INCREMENT PRIMARY KEY,
   nome VARCHAR(40) NOT NULL,
   nota VARCHAR(5)
)";

// executando um m�todo de $conexao
if ($conexao-&gt;query($sql) === TRUE) {
    echo "Tabela criada com sucesso!&lt;br&gt;";
} else {
    // acessando a propriedade error de $conexao
    echo "Erro na cria��o da tabela: " . $conexao-&gt;error; 
}

// m�todo do objeto $conexao
$conexao-&gt;close();
?&gt;
</pre>
</div>
</div>

<div id="outline-container-org8eb62e0" class="outline-3">
<h3 id="org8eb62e0"><span class="section-number-3">2.7</span> Exerc�cio 3</h3>
<div class="outline-text-3" id="text-2-7">
<p>
Criar as Tabelas:
</p>

<ul class="org-ul">
<li>pessoas (nome, email, senha)</li>
<li>listas (nome, id_pessoa, estado)</li>
<li>itens (nome, id_lista, estado) *</li>
<li>compartilhar (id_lista, id_pessoa)</li>
</ul>

<p>
Todas as tabelas possuem a coluna <b>id</b>. 
<b>id_pessoa</b> faz a liga��o entre listas e pessoas.
<b>id_lista</b> faz a liga��o entre itens e listas.
</p>

<p>
Veja o esquema das tabelas aqui:
</p>

<p>
<a href="https://dbdesigner.page.link/dQGk">https://dbdesigner.page.link/dQGk</a>
</p>
</div>
</div>

<div id="outline-container-orgc4d5ce6" class="outline-3">
<h3 id="orgc4d5ce6"><span class="section-number-3">2.8</span> Inserindo dados</h3>
<div class="outline-text-3" id="text-2-8">
<p>
Depois de criar o banco e a tabela podemos adicionar dados.
</p>

<p>
As regras s�o:
</p>

<ul class="org-ul">
<li>A consulta SQL deve ser escrita entre aspas.</li>
<li>Os valores que s�o string dentro da consulta devem aparecer entre ap�strofos</li>
<li>Valores num�ricos n�o devem ser colocados em ap�strofos</li>
<li>A palavra NULL n�o deve ser colocada entre ap�strofos</li>
</ul>

<p>
O comando abaixo � usado para inserir dados:
</p>

<pre class="example">
INSERT INTO nome_tabela (coluna1, coluna2, coluna3,...)
VALUES (valor1, valor2, valor3,...)
</pre>

<p>
Para inserir dados na tabela <b>alunos</b> temos o comando:
</p>

<pre class="example">
INSERT INTO alunos (nome, nota) VALUES ('Fulano', '5.5')
</pre>

<p>
Note que a nota aparece entre ap�strofos (') porque � armazenada em um campo com tipo VARCHAR.
</p>

<p>
Novamente a p�gina de inser��o de dados � bem parecida com a p�gina de cria��o de tabela.
</p>

<pre class="example">
&lt;?php
$servidor = "localhost";
$usuario = "root";
$senha = "toor";
$banco = "bdEscola"; // novo campo

// Cria a conex�o:
// Novo objeto!
$conexao = new mysqli($servidor, $usuario, $senha, $banco);

// Verifica a conex�o
// Atributo do objeto $conexao
if( $conexao-&gt;connect_error ) {
   die("A conex�o falhou: " . $conexao-&gt;connect_error());
}

echo "Conex�o realizada com sucesso!";

$sql = "INSERT INTO alunos (nome, nota) 
VALUES ('Fulano', '5.5')";

// executando um m�todo de $conexao
if ($conexao-&gt;query($sql) === TRUE) {
    echo "Aluno cadastrado!&lt;br&gt;";
} else {
    // acessando a propriedade error de $conexao
    echo "Erro no cadastro do aluno: " . $conexao-&gt;error; 
}

// m�todo do objeto $conexao
$conexao-&gt;close();
?&gt;
</pre>
</div>
</div>

<div id="outline-container-orgfbe751c" class="outline-3">
<h3 id="orgfbe751c"><span class="section-number-3">2.9</span> Criptografia</h3>
<div class="outline-text-3" id="text-2-9">
<p>
Podemos usar a fun��o <b>hash()</b> para criptografar utilizando um algoritmo. Para usar sha256 que produz 64 caracteres podemos usar:
</p>

<pre class="example">
$senha_normal = '123456';

$senha_criptografada = hash('sha256', $senha_normal);
</pre>

<p>
Se salvar $senha_criptografada no banco de dados, vai precisar utilizar a fun��o hash() antes na senha recebida do usu�rio para comparar com a salva no banco.
</p>
</div>
</div>


<div id="outline-container-orgaf2227c" class="outline-3">
<h3 id="orgaf2227c"><span class="section-number-3">2.10</span> Exerc�cio 4</h3>
<div class="outline-text-3" id="text-2-10">
<p>
Crie uma p�gina que cadastre o usu�rio. A senha deve ser criptografada antes de salvar no banco.
</p>
</div>
</div>

<div id="outline-container-org33908b5" class="outline-3">
<h3 id="org33908b5"><span class="section-number-3">2.11</span> Selecionando dados</h3>
<div class="outline-text-3" id="text-2-11">
<p>
Para selecionar dados usamos:
</p>

<pre class="example">
SELECT nomeColuna1, nomeColuna2 FROM nomeTabela
</pre>

<pre class="example">
&lt;?php
$servidor = "localhost";
$usuario = "root";
$senha = "toor";
$banco = "bdEscola"; // novo campo

// Cria a conex�o:
// Novo objeto!
$conexao = new mysqli($servidor, $usuario, $senha, $banco);

// Verifica a conex�o
// Atributo do objeto $conexao
if( $conexao-&gt;connect_error ) {
   die("A conex�o falhou: " . $conexao-&gt;connect_error());
}

echo "Conex�o realizada com sucesso!";

$sql = "SELECT nome, nota FROM alunos";

$result = $conn-&gt;query($sql);

if ($result-&gt;num_rows &gt; 0) {
    // mostrar cada linha da tabela
    while($linha = $result-&gt;fetch_assoc()) {
        echo "Nome: " . $linha['nome'] . " Nota: " . $linha['nota'] . "&lt;br&gt;";
    }
} else {
    echo "Nenhum aluno";
}

// m�todo do objeto $conexao
$conexao-&gt;close();
?&gt;

</pre>
</div>
</div>

<div id="outline-container-org728feec" class="outline-3">
<h3 id="org728feec"><span class="section-number-3">2.12</span> Exerc�cio 5</h3>
<div class="outline-text-3" id="text-2-12">
<p>
Crie uma p�gina de login para o usu�rio. Quando o usu�rio acerta o E-mail e senha voc� deve salvar o nome e o id dele na sess�o, exemplo:
</p>

<pre class="example">
$sql = "SELECT id, nome FROM pessoas WHERE senha = $senha_criptografada AND email = $email;

$_SESSION['nome'] = $linha['nome'];
$_SESSION['id'] = $linha['id'];
</pre>
</div>
</div>

<div id="outline-container-orgb09df94" class="outline-3">
<h3 id="orgb09df94"><span class="section-number-3">2.13</span> Exerc�cio 6</h3>
<div class="outline-text-3" id="text-2-13">
<p>
Crie a p�gina que cria uma lista, a p�gina deve verificar se o usu�rio est� logado:
</p>

<pre class="example">
isset($_SESSION['id'])
</pre>

<p>
Se o usu�rio estiver logado o usu�rio deve fornecer um nome para a lista e voc� deve armazenar o nome na tabela listas.
</p>
</div>
</div>

<div id="outline-container-orge93a97c" class="outline-3">
<h3 id="orge93a97c"><span class="section-number-3">2.14</span> Exerc�cio 7</h3>
<div class="outline-text-3" id="text-2-14">
<p>
Crie uma p�gina que mostra as listas criadas, quando o usu�rio seleciona uma lista voc� adiciona o id da lista na sess�o:
</p>

<pre class="example">
$_SESSION['id_lista'] = $lista_selecionada;
</pre>
</div>
</div>

<div id="outline-container-orgeb01153" class="outline-3">
<h3 id="orgeb01153"><span class="section-number-3">2.15</span> Exerc�cio 8</h3>
<div class="outline-text-3" id="text-2-15">
<p>
Crie uma p�gina que adiciona itens � lista selecionada no exerc�cio anterior. Lembre-se de usar o id da lista que est� gravado na sess�o. 
</p>
</div>
</div>

<div id="outline-container-orgd34fca4" class="outline-3">
<h3 id="orgd34fca4"><span class="section-number-3">2.16</span> Exerc�cio 9</h3>
<div class="outline-text-3" id="text-2-16">
<p>
Crie uma p�gina que permite o compartilhamento da lista atual com um dos usu�rios do sistema. O usu�rio digita o email do usu�rio com quem a lista ser� compartilhada.
</p>
</div>
</div>
</div>
</div>
<div id="postamble" class="status">
<p class="date">Created: 2019-10-01 ter 21:47</p>
<p class="validation"><a href="http://validator.w3.org/check?uri=referer">Validate</a></p>
</div>
</body>
</html>
