---
id: bad87fee1348bd9aeda08826
title: Target Elements by id Using jQuery
required:
  - link: 'https://cdnjs.cloudflare.com/ajax/libs/animate.css/3.2.0/animate.css'
challengeType: 6
videoUrl: ''
localeTitle: Elementos de destino por id usando jQuery
---

## Description
<section id="description"> Você também pode segmentar elementos por seus atributos id. Primeiro, direcione seu elemento <code>button</code> com o id <code>target3</code> usando o seletor <code>$(&quot;#target3&quot;)</code> . Note que, assim como com as declarações CSS, você digita um <code>#</code> antes do nome do id. Em seguida, use a função <code>.addClass()</code> do jQuery para adicionar as classes <code>animated</code> e <code>fadeOut</code> . Aqui está como você faria o elemento <code>button</code> com o id <code>target6</code> fade out: <code>$(&quot;#target6&quot;).addClass(&quot;animated fadeOut&quot;)</code> . </section>

## Instructions
<section id="instructions">
</section>

## Tests
<section id='tests'>

```yml
tests:
  - text: Selecione o elemento <code>button</code> com o <code>id</code> de <code>target3</code> e use a função jQuery <code>addClass()</code> para dar a classe de <code>animated</code> .
    testString: 'assert($("#target3").hasClass("animated"), "Select the <code>button</code> element with the <code>id</code> of <code>target3</code> and use the jQuery <code>addClass&#40&#41</code> function to give it the class of <code>animated</code>.");'
  - text: Segmente o elemento com o id <code>target3</code> e use a função jQuery <code>addClass()</code> para dar a classe <code>fadeOut</code> .
    testString: 'assert(($("#target3").hasClass("fadeOut") || $("#target3").hasClass("fadeout"))  && code.match(/\$\(\s*.#target3.\s*\)/g), "Target the element with the id <code>target3</code> and use the jQuery <code>addClass&#40&#41</code> function to give it the class <code>fadeOut</code>.");'
  - text: Use apenas o jQuery para adicionar essas classes ao elemento.
    testString: 'assert(!code.match(/class.*animated/g), "Only use jQuery to add these classes to the element.");'

```

</section>

## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("button").addClass("animated bounce");
    $(".well").addClass("animated shake");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
