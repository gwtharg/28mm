+++
title = "Flowcharts Notes"
date = 2020-04-07T13:07:35+01:00
weight = 5
chapter = true
pre = "<b>X. </b>"
+++

## Straight html

``` html
<div class="mermaid">
graph LR;
  A-->B;
</div>
```
<div class="mermaid">
graph LR;
  A-->B;
</div>
<script async src="https://unpkg.com/mermaid@8.2.3/dist/mermaid.min.js"></script>

<script async src="https://unpkg.com/mermaid@8.2.3/dist/mermaid.min.js"></script>

## Mermaid 
### not rendering yet!!!

{{<mermaid align="left">}}
graph LR;
    A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
{{< /mermaid >}}

## Used external website to create png

Rendering from local png files */content/markdown/flowcharts/name.png* as referenced from flowcharts.md file
### m1.png
![m1 png](./m1.png)
### m2.png 
![m2.png](./m2.png)

<hr>

## From online link

[![](https://mermaid.ink/img/eyJjb2RlIjoiXG5zZXF1ZW5jZURpYWdyYW1cbiAgICBwYXJ0aWNpcGFudCBBbGljZVxuICAgIHBhcnRpY2lwYW50IEJvYlxuICAgIEFsaWNlLT4-Sm9objogSGVsbG8gSm9obiwgaG93IGFyZSB5b3U_XG4gICAgbG9vcCBIZWFsdGhjaGVja1xuICAgICAgICBKb2huLT5Kb2huOiBGaWdodCBhZ2FpbnN0IGh5cG9jaG9uZHJpYVxuICAgIGVuZFxuICAgIE5vdGUgcmlnaHQgb2YgSm9objogUmF0aW9uYWwgdGhvdWdodHMgPGJyLz5wcmV2YWlsLi4uXG4gICAgSm9obi0tPkFsaWNlOiBHcmVhdCFcbiAgICBKb2huLT5Cb2I6IEhvdyBhYm91dCB5b3U_XG4gICAgQm9iLS0-Sm9objogSm9sbHkgZ29vZCFcblx0XHRcdFx0XHQiLCJtZXJtYWlkIjp7InRoZW1lIjoiZGVmYXVsdCJ9LCJ1cGRhdGVFZGl0b3IiOmZhbHNlfQ)](https://mermaid-js.github.io/mermaid-live-editor/#/edit/eyJjb2RlIjoiXG5zZXF1ZW5jZURpYWdyYW1cbiAgICBwYXJ0aWNpcGFudCBBbGljZVxuICAgIHBhcnRpY2lwYW50IEJvYlxuICAgIEFsaWNlLT4-Sm9objogSGVsbG8gSm9obiwgaG93IGFyZSB5b3U_XG4gICAgbG9vcCBIZWFsdGhjaGVja1xuICAgICAgICBKb2huLT5Kb2huOiBGaWdodCBhZ2FpbnN0IGh5cG9jaG9uZHJpYVxuICAgIGVuZFxuICAgIE5vdGUgcmlnaHQgb2YgSm9objogUmF0aW9uYWwgdGhvdWdodHMgPGJyLz5wcmV2YWlsLi4uXG4gICAgSm9obi0tPkFsaWNlOiBHcmVhdCFcbiAgICBKb2huLT5Cb2I6IEhvdyBhYm91dCB5b3U_XG4gICAgQm9iLS0-Sm9objogSm9sbHkgZ29vZCFcblx0XHRcdFx0XHQiLCJtZXJtYWlkIjp7InRoZW1lIjoiZGVmYXVsdCJ9LCJ1cGRhdGVFZGl0b3IiOmZhbHNlfQ)
