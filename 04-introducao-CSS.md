## Introducao ao CSS

> CSS = Cascading Style Sheets (Folha de Estilo em Cascata)

> CSS é uma <b>linguagem de estilos</b>
>> <b> Não é </b> uma linguagem de programação, nem  linguagem de marcação

## Formas de declaração

São definidos na seguinte forma:  
*propriedade: valor;*


### CSS inline

Incluido na própria linha usando a propriedade *style*

```html
<h2 style="background: rgba(221, 252, 110, 0.836); color:rgb(123, 63, 202)">CSS inline tem prioridade sobre outras formas de estilo </h2>
```

### CSS interno

Definindo no head dentro da tag *style*

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

### CSS externo

1. Criar um arquivo externo `./assets/css/style.css`

```css
h1 {
    background: rgba(49, 160, 127, 0.692);
    color: rgb(19, 78, 156);
}
```

2. Incluir o arrquivo no head usando a tag `<link>`

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trilha de CSS</title>
    <link rel="stylesheet" href="./assets/css/style.css">
</head>
```
</details>