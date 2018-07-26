# Curso Básico de CSS - 1 Atualização

https://www.schoolofnet.com/curso-css-basico/

---

## <a name="indice">Índice</a>

- [Introdução](#parte1)   
- [Seletores](#parte2)   
- [Prioridade dos seletores](#parte3)   
- [Seletores dentro de seletores e display](#parte4)   
- [Links](#parte5)   
- [Estilizando formulários](#parte6)   
- [Trabalhando com botões](#parte7)   
- [Fontes e CSS externo](#parte8)   

---

## <a name="parte1">Introdução</a>

```html
<!DOCTYPE html>
<html lang="pt-br">
    <head>
        <title></title>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <link href="css/style.css" rel="stylesheet">
    </head>
    <body>
        <h1 style="color:red">Sou título principal</h1>
        <p style="color: dodgerblue">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas elementum, felis vel ultricies facilisis, elit justo commodo
            diam, accumsan eleifend massa arcu et nulla. Integer facilisis dolor eget imperdiet commodo. Ut eu porta risus. Quisque
            sit amet gravida justo. Nunc luctus scelerisque erat at vestibulum. Integer posuere sem sed lorem cursus eleifend. Phasellus
            in congue urna, in rhoncus elit. In ullamcorper justo nec lacus condimentum, at placerat nisl venenatis. Quisque et diam
            sapien. Etiam consectetur commodo sapien. Praesent condimentum eget massa sed hendrerit. Nulla facilisi.</p>

    </body>
</html>
```

[Voltar ao Índice](#indice)

---

## <a name="parte2">Seletores</a>

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <title></title>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <style>
        h1 {
            color: red;
        }

        #redh1 {
            color: brown
        }

        p {
            color: orchid;
        }

        .blue {
            color: blue;
        }
        .yeloow{
            color: yeloow;
        }
    </style>
</head>

<body>
    <h1>Sou título principal</h1>

    <h1 id="redh1">Sou título principal</h1>

    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas elementum, felis vel ultricies facilisis, elit justo
        commodo diam, accumsan eleifend massa arcu et nulla. Integer facilisis dolor eget imperdiet commodo. Ut eu porta
        risus. Quisque sit amet gravida justo. Nunc luctus scelerisque erat at vestibulum. Integer posuere sem sed lorem
        cursus eleifend. Phasellus in congue urna, in rhoncus elit. In ullamcorper justo nec lacus condimentum, at placerat
        nisl venenatis. Quisque et diam sapien. Etiam consectetur commodo sapien. Praesent condimentum eget massa sed hendrerit.
        Nulla facilisi.
    </p>

    <p class="blue">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas elementum, felis vel ultricies facilisis, elit justo
        commodo diam, accumsan eleifend massa arcu et nulla. Integer facilisis dolor eget imperdiet commodo. Ut eu porta
        risus. Quisque sit amet gravida justo. Nunc luctus scelerisque erat at vestibulum. Integer posuere sem sed lorem
        cursus eleifend. Phasellus in congue urna, in rhoncus elit. In ullamcorper justo nec lacus condimentum, at placerat
        nisl venenatis. Quisque et diam sapien. Etiam consectetur commodo sapien. Praesent condimentum eget massa sed hendrerit.
        Nulla facilisi.
    </p>

    <p class="blue">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas elementum, felis vel ultricies facilisis, elit justo
        commodo diam, accumsan eleifend massa arcu et nulla. Integer facilisis dolor eget imperdiet commodo. Ut eu porta
        risus. Quisque sit amet gravida justo. Nunc luctus scelerisque erat at vestibulum. Integer posuere sem sed lorem
        cursus eleifend. Phasellus in congue urna, in rhoncus elit. In ullamcorper justo nec lacus condimentum, at placerat
        nisl venenatis. Quisque et diam sapien. Etiam consectetur commodo sapien. Praesent condimentum eget massa sed hendrerit.
        Nulla facilisi.
    </p>

</body>

</html>
```

[Voltar ao Índice](#indice)

---

## <a name="parte3">Prioridade dos seletores</a>

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <title></title>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <style>
        p {
            color: green;
        }

        .yellow {
            color: yellow;
        }

        .blue {
            color: blue;
        }

        #red {
            color: red;
        }
    </style>
</head>

<body>
<h1 >Sou título principal</h1>

<p class="yellow" id="red">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas elementum, felis vel ultricies
    facilisis, elit
    justo
    hendrerit.
    Nulla facilisi.
</p>

<p> cursus eleifend. Phasellus in congue urna, in rhoncus elit. In ullamcorper justo nec lacus condimentum, at placerat
    nisl venenatis. Quisque et diam sapien. Etiam consectetur commodo sapien. Praesent condimentum eget massa sed
    hendrerit.
    Nulla facilisi.
</p>

<p class="blue">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas elementum, felis vel ultricies
    facilisis, elit justo
    commodo diam, accumsan eleifend massa arcu et nulla. Integer facilisis dolor eget imperdiet commodo. Ut eu porta
    risus. Quisque sit amet gravida justo. Nunc luctus scelerisque erat at vestibulum. Integer posuere sem sed lorem
    hendrerit.
    Nulla facilisi.
</p>


</body>

</html>
```

[Voltar ao Índice](#indice)

---

## <a name="parte4">Seletores dentro de seletores e display</a>

```css

        .nav ul li{
            display: inline-block;
        }

        nav ul{
            padding: 0;
        }
```

```html
<nav class="nav">
    <ul>
        <li><a href="">Home</a></li>
        <li><a href="">Sobre Nós</a></li>
        <li><a href="">Produtos</a></li>
        <li><a href="">Contato</a></li>
    </ul>
</nav>
```


[Voltar ao Índice](#indice)

---

## <a name="parte5">Links</a>


[Voltar ao Índice](#indice)

---

## <a name="parte6">Estilizando formulários</a>


[Voltar ao Índice](#indice)

---

## <a name="parte7">Trabalhando com botões</a>


[Voltar ao Índice](#indice)

---

## <a name="parte8">Fontes e CSS externo</a>


[Voltar ao Índice](#indice)

---
