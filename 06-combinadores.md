# Combinadores CSS

## Agrupamento de seletores

```css
li,
ul,
fieldset {
    background-color: rgb(137, 215, 221);
}
```

## Combinador descendente
 
 ```css
 li li {
    color: rgb(39, 145, 29)
}
 ```

 ```css
 
 #lista-01 li{
    color: rgb(39, 145, 29)
 }
 ```

 ## Combinador filho

Seleciona só a tag `<p>` filha, exclui as netas.

 ```css 
 div > p {
    color: red;
 }
 ```

 ## Combinador irmão

 ### Irmão adjacente 
 
 Aplica a tag posta ao lado.

 ```css
  div + p {
    color: red;
 }
 ```

 ### Irmão geral

 ```css
  div ~ p {
    color: red;
 }
 ```

 


