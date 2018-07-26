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

```css
     background-color: red;
            border: 3px solid darkred;
            color: white;
            padding: 10px;
            margin: 10px;
            display: inline-block;
            text-decoration: none;
        }
        .nav ul li a:hover{
            background-color: indianred;
            border: 3px solid red;
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

## <a name="parte6">Estilizando formulários</a>

```css
    form{
            border: dashed 2px green;
            padding: 20px;
        }
        input{
            display: block;
            width: 100%;
            margin: 0 0 10px 0;
            border: 1px solid #abc;
        }
```

```html
<form action="">
    <input type="text" placeholder="campo tipo texto">
    <input type="email" placeholder="campo tipo email">
    <input type="number" placeholder="campo tipo numer">
    <input type="date" placeholder="campo tipo data">
    <button>Salvar</button>
</form>

```


[Voltar ao Índice](#indice)

---

## <a name="parte7">Trabalhando com botões</a>

```css

        .btn {
            border-style: solid;
            border-top-width: 2px;
            border-bottom-width: 4px;
            border-left-width: 2px;
            border-right-width: 4px;
            color: white;
            cursor: pointer;
            display: inline-block;
            margin: 10px;
            padding: 10px;
            text-decoration: none;
            border-radius: 10px;
        }

        .btn-red {
            background-color: red;
            border-color: darkred;
        }

        .btn-red:hover {
            background-color: indianred;
            border-color: red;
        }

        .btn-blue {
            background-color: dodgerblue;
            border-color: deepskyblue;
        }

        .btn-blue:hover {
            background-color: lightskyblue;
            border: 3px solid;
            border-color: cornflowerblue;
        }

```

```html

<nav class="nav">
    <ul>
        <li><a href="" class="btn btn-red">Home</a></li>
        <li><a href="" class="btn btn-red">Sobre Nós</a></li>
        <li><a href="" class="btn btn-red">Produtos</a></li>
        <li><a href="" class="btn btn-red">Contato</a></li>
    </ul>
</nav>

<form action="">
    <input type="text" placeholder="campo tipo texto">
    <input type="email" placeholder="campo tipo email">
    <input type="number" placeholder="campo tipo numer">
    <input type="date" placeholder="campo tipo data">
    <button class="btn btn-blue">Salvar</button>
</form>


```

[Voltar ao Índice](#indice)

---

## <a name="parte8">Fontes e CSS externo</a>

- https://fonts.google.com/

```css
body{
    font-family: 'Fira Sans', sans-serif;
}

```

[Voltar ao Índice](#indice)

---
