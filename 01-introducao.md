# Introdução ao HTML

## Estrutura básica de uma página em HTML

```
<html>
  <title> 
    Título da página. O que está aqui não aparece na página 
  </title>
  <body>
    Corpo da página. Tudo aqui é o que aparece na página.
  </body>
</html>
```

## Tags

Algumas tags precisam ser abertas e fechadas, como é o caso de `<i>texto</i>`. Mas outras, por si só, já é um campo, como `<input>`.

Tag | Descrição
--- | ---
`<i> itálico </i>`           | <i> itálico </i>
`<strong> negrito </strong>` | <strong> negrito </strong>
`<u>sublinhado</u>`          |  <u>sublinhado</u>
`<input type="text" />`      | Cria um campo para digitação  <input type="text" />
`<img />`   | Insere imagem


## Atributos das Tags

São informações adicionais que definem o comportamento, estilo ou características específicas de elementos na página web.

- `id` cria uma identificacão para aquela tag

```
<strong id="texto"> Um texto que possui uma identificação </strong>
```
> <strong id="texto"> Um texto que possui uma identificação </strong>


- `class` define uma classe, onde, tudo o que for marcada como sendo daquela classe, terá a mesma formatação.

```
<i class="titulo-principal"> Texto classificado como título principal </strong>
```

> <i class="titulo-principal"> Texto classificado como título principal </i>

- `type` define o tipo do campo `input`

```
Campo de texto <input type="text" /> 
Campo numérico <input type="number" />
Seletor de cor <input type="color" />
```      
> Campo de texto <input type="text" />

> Campo numérico <input type="number" />

> Seletor de cor <input type="color" />

- `style` insere comandos css 
```
<strong style="color: blue"> Um texto azul </strong>
```
> <strong style="color: blue"> Um texto azul </strong>

- `src=""` indica o localização da imagem, e `width = ""` determina o tamanho da imagem 

```
<img src='https://u3r3f6s2.rocketcdn.me/wp-content/uploads/2021/01/image-32.png' width = "300"/>
```   
<img src='https://u3r3f6s2.rocketcdn.me/wp-content/uploads/2021/01/image-32.png' width = "300"/>

## Texto

```
<h1> Título 1 </h1>

<h2> Título 2 </h2>

<h3> Título 3 </h3>

<h4> Título 4 </h4>

<h5> Título 5 </h5>

<h6> Título 6 </h6>
```

```
<p>Isso é um parágrafo</p>
``` 
<p>Isso é um parágrafo</p>

```
<blockquote>
   Isso é uma citação/observação
</blockquote>

```
<blockquote>
   Isso é uma citação/observação
</blockquote>

##  Listas 

### Lista ordenada:

```
<ol> 
   <li> Item 1 </li>
   <li> Item 2 </li>
   <li> Item 3  
      <ol> 
         <li> Item 3.1 </li>
      </ol>
   </li>
</ol>
```

<ol> 
   <li> Item 1 </li>
   <li> Item 2 </li>
   <li> Item 3  
      <ol> 
         <li> Item 3.1 </li>
      </ol>
   </li>
</ol>

### Lista não ordenada

```
<ul> 
   <li> Item 1 </li>
   <li> Item 2 </li>
   <li> Item 3  
      <ul> 
         <li> Item 3.1 </li>
      </ul>
   </li>
</ul>

```

<ul> 
   <li> Item 1 </li>
   <li> Item 2 </li>
   <li> Item 3  
      <ul> 
         <li> Item 3.1 </li>
      </ul>
   </li>
</ul>

## Links

- Link abrindo n mesma janela:
```
<a href="https://github.com/anapppp"> Github da Ana  </a>
```

<a href="https://github.com/anapppp"> Github da Ana  </a>

- Link abrindo em uma nova aba:

```
<a href="https://github.com/anapppp" target="_blank"> Github da Ana</a>
```

<a href="https://github.com/anapppp" target="_blank"> Github da Ana</a>

- Link com balãozinho (*tooltip*):

```
<a href="https://github.com/anapppp" title="esse é o bão!"> Github da Ana</a>
```

<a href="https://github.com/anapppp" title="esse é o bão!"> Github da Ana</a>

> A tag `<a>` é chamada âncora
