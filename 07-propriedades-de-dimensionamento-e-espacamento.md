# Propriedades de dimensionamento e espaçamento

## Largura e altura

```css
div{
    width: 200px;
    height: 100px;
}
```


```css
div{
    min-width: 200px;
    max-height: 100px;
}
```

## Margin

```css
div{
    margin: 100px;
}
```

```css
div{
    margin-top: 100px;
    margin-bottom: 50px;
    margin-left: -20px;
    margin-right: -40px;
}
```

## Padding

Marca um espaçamento interno.

```css
div {
    padding: 100px
}
```

## Box Sizing

```css
div {
    box-sizing: border-box /*ajusta a altura e a largura desconsiderando o tamanho do padding*/
}
```

## Palavras reservadas

- `inherit`: especifica que uma propriedade deve herdar o valor de seu elemento pai.
- `auto`: frequentemente usada para propriedades que envolvem dimensionamento automático, como largura ou altura. 
- `initial`: Define uma propriedade para o seu valor inicial.
- `unset`: Reseta uma propriedade para seu valor inicial, mas se não houver um valor inicial, ele se comporta como `inherit`.
- `revert`: Volta para o valor da propriedade como se não houvesse regras aplicadas no nível do usuário. Funciona como uma combinação de `inherit` e `initial`.
