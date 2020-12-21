# Selectors

Conecta um elemento HTML com o CSS

## Tipos

* Global Selector `*`
* Element/Type Selector `h1, h2, p, div`
* ID Selector `#boz, #container`
* Class Selector `.red, .m-4`
* Attribute Selector, Pseudo-class, Pseudo-element, e outros

### Global Selector

```css
/* Neste caso irá pegar todos os elementos e deixa-los sem margens*/

* {
  margin: 0;
}
```

### Element/Type Selector

```css
/* Neste caso só o h1 irá receber as propriedades que estamos declarando */

h1 {
  color: green;
  font-size: 60px;
  background-color: gray;
}
```

### ID Selector

```html
<div id="container">
  <h1>Título</h1>  
</div>

<div>
  <h1>Exemplo</h1>  
</div>
```

```css
/* Neste caso apenas os elemento que tiverem o ID container sofreram mudanças */

#container {
  width: 200px;
  padding: 20px;
}
```

### Class Selector

```html
<div id="container">
  <h1>Título</h1>  
</div>

<div class="m-40">
  <h1>Exemplo</h1>  
</div>
```

```css
/* id */
#container {
  width: 200px;
  padding: 20px;
}

/* class */
.m-40 {
  margin: 40px;
}
```

### Agrupando Selectors

```html
<div>
  <h1>Título</h1>
  <h2>Subtítulo</h2>
</div>
```

```css
h1, h2{
  color: green;
  font-size: 60px;
  background-color: gray;
}
```
