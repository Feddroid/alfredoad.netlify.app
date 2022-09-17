# codeable-ui-c8


```html
<!-- etiqueta de apertura  -->
<!-- Contentido -->
<!-- Etiqueta de cierre -->
<!-- en conjunto hace un elemento -->
    <h1>content</h1> => element
```

Como darle formato.

- Ctrol + P
- Escribo ">"
- despues "Format document
- elijo Prettier y Enter.

## Image

### attributes
`src` => source
`alt` => alternative => muestra un texto alternativo si la imagen no carga.

accessibility => `a11y HTML`

# CSS
Cascading Style Sheets

## Selectors

```html
<style>
  /* selector {
      property: value;
    } */
  
    /* Selector by tags => h1 | p | li | ...  */
    h1 {
      color: tomato;
    }
    p {
      color: darkorange;
    }
    p {
      color: yellow;
    }
  
    /* Selector by class */
    .completed {
      color: green;
    }
  
    /* Selectro by id */
    #lorem {
      color: blue;
    }

    /* Selector global */
    * {
      color: aqua
    }

    /* Selector by tags => h1 | p | li | ...  */
    h1, h2, h3, h4, h5, p, .completed, #lorem {
      color: tomato;
    }

</style>
```

<!-- Font weight -->
```
100 Thin
200 Extra Light
300 Light
400 Normal
500 Medium
600 Semi Bold
700 Bold
800 Extra Bold
900 Ultra Bold
```


<!-- Propuesta de hacer submenu -->

```html
<li class="menu">
  <a href="#" class="link text semibold">Portafolio</a>
  <ul class="sub_menu list-style-none">
    <li><a href="#">List 1</a></li>
    <li><a href="#">List 2</a></li>
    <li><a href="#">List 3</a></li>
  </ul>
</li>
```

```css
.menu {
  position: relative;
}

.sub_menu {
  position: absolute;
  right: 0;
  padding: .5em;
  background-color: var(--green-800);
}

.sub_menu a {
  text-decoration: none;
  color: white;
}
```

# How to use `rebase`

```
$(current_branch): git rebase main

<!-- After conflic solution in VSCode -->

<!-- Ciclo de correccion de error - START -->

$(current_branch): git add .  #Sobrescribe el commit donde ocurrio el conflicto.

$(current_branch): git rebase --continue #si es que esto falla, usar el de abajo 👇

$(current_branch): git rebase --skip

<!-- Ciclo de correccion de error - END -->

$(current_branch): git push origin +current_branch  #(+) == --force
```
