# Seletores CSS

## Seletor de Tag

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trilha de CSS</title>
    <style>
        h2 {
            background: black;
            color: rgb(164, 77, 190);
        }
    </style>
</head>
```


## Seletor de ID

```html
<body>
    <p> Parágrafo com estilo definido para todos os parágrafos.</p>
    <p id="seletor-id"> Parágrafo com estilo definido pelo <b>Seletor de ID</b>. </p>
</body>
```

No arquivo *style.css*:
```css
p {
    background: rgba(2, 0, 22, 0.692);
    color: rgb(188, 212, 243);
}

#seletor-id {
    color: rgba(2, 0, 22, 0.692);
    background: rgb(188, 212, 243);
}
```

## Seletor de Class

Define estilos em varios elementos de uma só vez.

```html
<body>
    <ul>
        <li> Uma linha </li>
        <li> Outra linha </li>
        <li class="seletor-class">Uma linha defnida pelo seletor class </li>
        <li> Outra linha </li>
        <li class="seletor-class">Outra linha definida pela mesma classe </li>
        <li> Outra linha </li>
        <li class="seletor-class seletor-uppercase">Outra linha definida pela mesma classe, com mais uma classe sobreposta </li>
    </ul>
</body>
```

No arquivo *style.css*:

```css
.seletor-class {
    color: rgb(167, 135, 204);
    background-color: black;
}

.seletor-uppercase {
    text-transform: uppercase;
}
```

> classes podem se repetir, IDs não.

## Seletor Universal

Define as propriedades mais gerais da página.

```css
* {
    font-family: 'Courier New', Courier, monospace;
    background-color: rgb(239, 255, 248);
}
```

## Seletor de atributo

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Seletor de Atributo</title>
  <style>
    /* Este é o seletor de atributo */
    [type="text"] {
      border: 2px solid #3498db;
      padding: 5px;
    }
  </style>
</head>
<body>
  <label for="username">Este é um seetor de atributo:</label>
  <input type="text" id="username" name="username">
</body>
</html>
```