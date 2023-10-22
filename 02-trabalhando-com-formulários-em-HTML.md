# Trabalhando com Formulários em HTML

Como fazer para um formulario chegar no *backend*? 

## Tag `<form>`

Criando um formulário:

```
<form name="signup" method="POST" onsubmit="alert('Formulário enviado!')" target="_blank" action="enderecodomeusite">
Nome: <input type="text" name="NAME">

Idade: <input type="number" name="age">

Senha: <input type="password" name="password">

<button type="submit">Enviar</button>
</form>
```

<form name="signup" method="POST" onsubmit="alert('Formulário enviado!')" target="_blank" action="enderecodomeusite">
Nome: <input type="text" name="NAME">

Idade: <input type="number" name="age">

Senha: <input type="password" name="password">

<button type="submit">Enviar</button>
</form>

> Quando essas informações são enviadas para o backend, elas são identificados com o nome escrito em `name=""` 

> O `method="GET"` envia todos os campos do formulario como variveis na URL

> O `method="POST"` envia todos os campos do formulario no corpo da requisição HTTP (*body*)

> `target="_blank"` abre uma nova janela

> Em HTML, tudo que começa com `on` é um evento. Exemplo: `onclick`, `onsubmit` 

>> `onsubmit` permite inserir um código JavaScript.


## Tag `<input>`

[Aqui](https://www.w3schools.com/tags/tag_input.asp) tem uma lista completa dos atributos da tag `input`.
> O comando `<br>` pula a linha



```
<label> Campo de texto: </label> <input type="text" /><br>
```
<label> Campo de texto: </label> <input type="text" /><br>

```
<label> Campo numérico: </label> <input type="number" /><br>
```
<label> Campo numérico: </label> <input type="number" /><br>

```
<label> Seletor de cor: </label> <input type="color" /><br>
```
<label> Seletor de cor: </label> <input type="color" /><br>

```
<label> Seletor de intervalo: </label> <input type="range" /><br>
```
<label> Seletor de intervalo: </label> <input type="range" /><br>

```
<label> E-mail: </label> <input type="email" /><br>
```
<label> E-mail: </label> <input type="email" /><br>

```
<label> URL: </label> <input type="url" /><br>
```
<label> URL: </label> <input type="url" /><br>

```
<label> Data: </label> <input type="date" /><br>
```
<label> Data: </label> <input type="date" /><br>

```
<label> Mês: </label> <input type="month" /><br>
```
<label> Mês: </label> <input type="month" /><br>

```
<label> Checkbox: </label> <input type="checkbox" /><br>
```
<label> Checkbox: </label> <input type="checkbox" /><br>

```
<label> Radio: </label> <input type="radio" /><br>
```
<label> Radio: </label> <input type="radio" /><br>

```
<label> Campo invisível: </label> <input type="hidden" /><br>
```
<label> Campo invisível: </label> <input type="hidden" /><br>

```
<label> Envio de um arquivo: </label> <input type="file" /><br>
```
<label> Envio de um arquivo: </label> <input type="file" /><br>

```
<label> Envio de vários arquivos: </label> <input type="file" multiple /><br>
```
<label> Envio de vários arquivos: </label> <input type="file" multiple /><br>

```
<label> Busca: </label> <input type="search" /><br>
```
<label> Busca: </label> <input type="search" /><br>

```
<label> Botão: </label> <input type="submit" value="Botão" /><br>
```
<label> Botão: </label> <input type="button" value="Botão" /><br>


## Alguns cuidados com Checkbox e Ratio

O jeito certo de enviar o checkbox é com ` method="POST" ` e com `name` de todas as opcoes como "opcional[]", <u>indicando para o backend que se trata de uma lista</u>.

```
<label> Opcionais:</label><br>
<input type="checkbox" name="opcional[]" value="cebola"/>cebola<br>
<input type="checkbox" name="opcional[]" value="tomate"/>tomate<br>
<input type="checkbox" name="opcional[]" value="queijo"/>queijo<br>
```

<label> Opcionais:</label><br>
<input type="checkbox" name="opcional[]" value="cebola"/>cebola<br>
<input type="checkbox" name="opcional[]" value="tomate"/>tomate<br>
<input type="checkbox" name="opcional[]" value="queijo"/>queijo<br>


Já o radio não permite marcar mais de um campo. O `name` também precisa ser igual.

```
<label> Deseja borda recheada?</label><br>
<input type="radio" name="borda" value="sim"/>Sim<br>
<input type="radio" name="borda" value="nao"/>Não<br>
```

<label> Deseja borda recheada?</label><br>
<input type="radio" name="borda" value="sim"/>Sim<br>
<input type="radio" name="borda" value="nao"/>Não<br>

## Button e seus tipos

```
<label> Botão simples : </label> <input type="button" value="Botao Simples" onmouseOver="alert('Esse botão não faz nada')" /><br>
```
<label> Botão simples : </label> <input type="button" value="Botao Simples" onmouseOver="alert('Esse botão não faz nada')" /><br>

```
<label> Reset: </label> <input type="reset" value= "Limpar formulário" title="Limpa todo o <form> no qual o botao está contido"/><br>
```
<label> Reset: </label> <input type="reset" value= "Limpar formulário" title="Limpa todo o <form> no qual o botao está contido"/><br>

```
<label> Enviar formulário: </label> <input type="submit" value= "Enviar formulário" title="Envia o <form> no qual o botao está contido" /><br>
```
<label> Enviar formulário: </label> <input type="submit" value= "Enviar formulário" title="Envia o <form> no qual o botao está contido" /><br>


## Select e seus tipos
Selecionar uma única opção:
```
<label> Selecionar: </label>
<select name="opcao">
<option value="opcao0" selected>Sem solução</option>
<option value="opcao1">A melhor opção</option>
<option value="opcao2">Opção bem melhor do que a anterior</option>
<option value="opcao3">Melhor opção de todas</option>
</select><br>
```

<label> Selecionar: </label>
<select name="opcao">
<option value="opcao0" selected>Sem solução</option>
<option value="opcao1">A melhor opção</option>
<option value="opcao2">Opção bem melhor do que a anterior</option>
<option value="opcao3">Melhor opção de todas</option>
</select><br>

Selecionar múltiplas opções:

```
<label> Selecionar: </label>
<select name="opcao" multiple>
<option value="opcao0" selected>Sem solução</option>
<option value="opcao1">A melhor opção</option>
<option value="opcao2">Opção bem melhor do que a anterior</option>
<option value="opcao3">Melhor opção de todas</option>
</select><br>
```

<label> Selecionar: </label>
<select name="opcao" multiple>
<option value="opcao0" selected>Sem solução</option>
<option value="opcao1">A melhor opção</option>
<option value="opcao2">Opção bem melhor do que a anterior</option>
<option value="opcao3">Melhor opção de todas</option>
</select><br>

## Textarea

É uma tag para criar uma área de texto.
```
<label> Escreva um texto: </label>
<textarea rows="2" cols="80" name="texto" >
</textarea><br>
```

<label> Escreva um texto: </label>
<textarea rows="2" cols="80" name="texto" >
</textarea><br>