# A Cascata (cascading)

A escolha de browser de qual regra aplicar, caso haja muitas regras para o mesmo elemento.

* Seu estilo é lido de cima para baixo.

Vamos usar como exemplo estes códigos:

```html
<!-- código HTML -->
<h1>Título</h1>
```

```css
/* código CSS */
h1 {
  color: red;
}

h1 {
  color: blue;
}

/* a cor final do h1 será blue, pois estamos lendo os estilos de cima para baixo e a ultima coisa que é feita no h1 é colocar sua cor como blue */
```

É levado em consideração 3 fatores

1. Origem do estilo
2. Especificidade 
3. Importância 

============================

### Origem do estilo

inline > tag style > tag link 

- A estilização inline é a mais forte, a que irá prevalecer

============================

### Especificidade 

É um cálculo matemático, onde, cada tipo de seletor e origem do estilo, possuem valores a serem considerados.

0. Universal selector, combinators e negation pseudo-class (:not())
1. Element type selector e pseudo-elements (::before, ::after)
10. Classes e attribute selectors ([type="radio"])
100. ID selector
1000. Inline

============================

### A regra !important

* cuidado, evite o uso
* não é considerado uma boa prática
* quebra o fluxo natural da cascata 

```css
h1 {
    color: blue !important;
}

h1 {
    color: red;
}

/* O !important é o mais forte, sempre será dada preferência as tags com !important */
```