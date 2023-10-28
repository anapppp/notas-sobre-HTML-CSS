# Estruturando seu HTML

## Mais algumas Tags

Tag | Descrição
--- | ---
`Texto <mark> destacado </mark>` | Texto <mark> destacado </mark>
`Texto <sup>superior</sup>` | Texto <sup>superior</sup>
`Texto <sub>inferior</sub>` | Texto <sub>inferior</sub>
`<font color="red"> Texto vermelho </font>` | <font color="red"> Texto vermelho </font>
`<font face="Times New Roman"> Texto em Times New Roman </font>` | <font face="Times New Roman"> Texto em Times New Roman </font>

> ⚠️ <font color="red"><strong>Atenção:</strong></font> ambas as tags `<b>` e `<strong>` deixam o texto em negrito, porém, quando é feito a leitura do texto por apps de acessibilidade, o comando `<strong>` enfatiza a leitura da palavra. <strong> Por isso é preferivel usar `<strong>` que `<b>` </strong>.

## Tags `<div>` e `<span>`

São tags que não possuem valor semântico.

<img width="300" src="https://i.stack.imgur.com/KvsHF.png"/>

A tag `<div>` ocupa a horizontal inteira, enquanto que a `<spam>` ocupa só o local.

## Tag `<fieldset>`
Delimita uma região.

```html
<fieldset>
    <legend> Dados pessoais: </legend>
</fieldset>
```
![image](https://github.com/anapppp/notas-sobre-HTML-CSS/assets/70073296/77b8ef22-5923-4c23-be35-5210ea9c7b6a)

## Iframes

Serve para colocar uma pagina dentro de uma pagina

```html
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d26598.48982729564!2d33.72024623144643!3d16.93740068290994!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x16864d9f7e080ffb%3A0xa128a0af2c7225e8!2sMero%C3%AB%20East%20(Main)%20Necropolis!5e0!3m2!1spt-BR!2sbr!4v1698463068647!5m2!1spt-BR!2sbr" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
```

## Cores

Acesse o [HTML Color Codes](https://htmlcolorcodes.com/).