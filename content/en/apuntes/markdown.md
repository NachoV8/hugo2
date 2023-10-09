+++
title = 'Markdown'
date = 2023-09-19T11:08:45+02:00
draft = false
+++

# Apuntes

#### Descargas

{{% attachments color="black" icon="fab fa-hackerrank" /%}}

#### colores


Como poner un título
```bash

#Titulo

```

Texto en negrita entre 2 * **bold text**

Para poner en cursiva entre _  _italicized text_

#### Lista

- Para hacer listas ponemos un guión delante
  - Si queremos tabulamos para asi poder hacer una sublista


#### Checkbox

- [x] Introducimos una x en la casilla que queramos marcar
- [ ] More Tests
  - [x] Hacemos lo mismo si queremos subcasillas

    
#### Tablas

| Option | Description |
|--------|-------------|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |


Poner link a una palabra
    [Google](http://google.es)


{{% button href="https://google.com/" icon="search" %}}Google{{% /button %}}

#### Código

   {{< highlight lineNos="true" lineNoStart="666" type="py" >}}
# the hardest part is to start writing code; here's a kickstart; just copy and paste this; it's free; the next lines will cost you serious credits
print("Hello")
print(" ")
print("World")
print("!")
{{< /highlight >}}


{{< highlight type="py" wrap="true" hl_lines="2" >}}
# Quicksort Python One-liner
lambda L: [] if L==[] else qsort([x for x in L[1:] if x< L[0]]) + L[0:1] + qsort([x for x in L[1:] if x>=L[0]])
# Some more stuff
{{< /highlight >}}

#### Expandir texto
{{% expand title="Leer más" %}}Con este shortcode podemos ocultar el texto y mostrarlo solo cuando queramos.{{% /expand %}}

#### Iconos
Añado un icono {{% icon icon="angle-double-up" %}}

#### Operaciones
Podemos poner operaciones matemáticas/químicas
{{< math >}}
$$\ce{Hg^2+ ->[I-] HgI2 ->[I-] [Hg^{II}I4]^2-}$$
{{< /math >}}

{{% include file="shortcodes/instalacion.md" %}}

#### Diagramas

Podemos realizar diagramas personalizados 

{{< mermaid zoom="true">}}
---
title: Titulo diagrama
---
graph LR;
    A[Instalar tree] -->|Despues| B(Instalamos apache2)
    B --> |1|C[Codigo abierto y gratuito]
    B --> |2|D[Multiplataforma]
    B --> |3|E[Parches de seguridad regulares]
{{< /mermaid >}}


#### Gráficos
  {{< mermaid zoom="false" >}}
pie title Tiempo de estudio
    "Entorno servidor" : 58
    "Entorno cliente" : 42
    "Empresa" : 20
{{< /mermaid >}}

#### Avisos

{{% notice style="warning" title="Aviso"%}}
Esto es un aviso para avisarte que hay un aviso
{{% /notice %}}


#### URL

`https://github.com/McShelby/hugo-theme-relearn/edit/main/exampleSite/content/` {{% siteparam name="" %}}

{{% tab title="_**Mixed**_" %}}
Podemos juntar texto y código en una misma tabla
```python
printf("Hello World!");
```
{{% /tab %}}