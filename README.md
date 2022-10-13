# Appunti

## Dimensioni tipo

Le dimensioni tipo sono [1050 x 700](https://quarto.org/docs/presentations/revealjs/advanced.html#presentation-size).

## Ridimensionamento automatico immagini

Impostare nel tema `auto-stretch: false`, in modo che le immagini piccole non si ridimensionino alla larghezza.

Si può pure impostare per slide, usando `## Slide Title {.nostretch}`

## Export file HTML univoco

È possibile generare un file HTML che ingloba tutto al suo interno. Per farlo aggiungere l'opzione `self-contained: true`.
Durante lo sviluppo è bene tenerla a `false`, altrimenti diventa pesante e lungo il *rendering*.

## Prima pagina con immagine di sfondo

Cancellare tutti i metadati, come titolo, autore, ecc. e inserire un background

```
# {background-color="black" background-image="risorse/prima-pagina.png" background-size="contain"}
```

## Inglobare un CSS

~~~
```{=html}
<style type="text/css">
caption, .table-caption {
  text-align: left;
}
</style>
```
~~~

Vedi: <https://github.com/quarto-dev/quarto-cli/discussions/1042#discussioncomment-2867731=>


## Centrare orizzontalmente

Usare `<center>`.

Ad esempio

```markdown
<center>
Ciao mondo
</center>
```

## Impostare dimensioni immagini

Aggiungere ad esempio `{height=500}` fisserà l'altezza in pixel, e la larghezza si adatterà in proporzione.
