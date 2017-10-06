Comandos pandoc
===============

````
pandoc 1.19.2.1
Compiled with pandoc-types 1.17.0.4, texmath 0.9, skylighting 0.1.1.4
Default user data directory: /Users/ovis/.pandoc
Copyright (C) 2006-2016 John MacFarlane
Web:  http://pandoc.org
This is free software; see the source for copying conditions.
There is no warranty, not even for merchantability or fitness
for a particular purpose.

```




Comandos
--------

### Para convertir de Markdown a Word, con documento de Word como plantilla:

Encontré esto:

`pandoc -f markdown -t docx --reference-docx reference_document.docx your_markdown_file.md -o destination_document.docx`



Cambiando por mis archivos:

`pandoc -f markdown -t docx --reference-docx plantilla_lancis.docx Protocolo_Presentaciones_LANCIS_v2.md -o Protocolo_Presentaciones_LANCIS_v2.docx`

- - -

### Para convertir de Markdown a HTML, con estilo CSS incoprporado al HTML:

Encontré:

`pandoc FILENAME.md -s -c TEMPLATECSS.css -o FILENAME.html`

donde `-s` es `--standalone`, `-c` es `--css` (debe ir seguido del url o del nombre del CSS a usar si está en la misma carpeta)

Sí funciona, pero el CSS debe estar en la misma carpeta cada vez que se abra el HTML. Para integrar el CSS al HTML hay que usar `--self-contained`. Corrió así:

`pandoc Protocolo_Presentaciones_LANCIS.md -s -c buttondown.css --self-contained -o Protocolo_Presentaciones_LANCIS.html`

> jottr commented on Sep 2, 2014
You can use css to convert to html. To convert to pdf from html you will either need to use wkhtmltopdf, or alternatively use a tex based template instead of css.
To convert to html you can do the following:

> `pandoc foo.md -s -c buttondown.css -o foo.html`

El CSS buttondown lo encontré en: [A clean, minimal CSS stylesheet for Markdown, Pandoc and MultiMarkdown HTML output.](https://gist.github.com/ryangray/1882525)

- - -
