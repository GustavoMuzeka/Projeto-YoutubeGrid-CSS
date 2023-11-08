# Projeto para o bootcamp da DIO sobre CSS


![YouTube Layout - Demo](./final/assets/img/demo.gif)

<hr>

    - Grid Lines
    - Grid Track
    - Grid Cell
    - Grid Area
<hr>


```CSS
    display: grid
    display: inline-grid
```


```CSS
    grid-template-columns: 50px 100px 200px;
    grid-template-rows: 100px 150px;
```


```CSS
    .e {
        grid-column-start: 1;
        grid-column-end: 3;
        grid-row-start: 1;
        grid-row-end: 2;
    }
```


```CSS
    .e {
        grid-column: 1 / 4;
        grid-row: 1 / 2;
    }

    .d {
        grid-area: 1 / 1 / 2 / 3;
    }
```


```CSS
    grid-column-gap: 10px;
    grid-row-gap: 20px;

    grid-gap: 10px 20px;

    grid-gap: 20px;
```


```CSS
    grid-template-areas:
        "header header header"
        "nav content aside"
        "footer footer footer";

    grid-area: header;
    grid-area: nav;
    grid-area: content;
    grid-area: aside;
    grid-area: footer;

/* Responsive Web Design */

@media(max-width: 590px) {
    .grid-container {
        grid-template-columns: 25% 75%;
        grid-template-rows: 20% 10% 50% 20%;
        grid-template-areas:
        "header header"
        "nav nav"
        "content aside"
        "footer footer";
    }
}

    @media(max-width: 450px) {
    .grid-container {
        grid-template-columns: 100%;
        grid-template-rows: 20% 10% 10% 50% 10%;
        grid-template-areas:
        "header"
        "nav"
        "content" 
        "aside"
        "footer";
    }
}
```
<hr>

