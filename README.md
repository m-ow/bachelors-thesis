## Una prueba transicional de la confluencia de la reducción η

Tesis de licenciatura de Maximiliano Onofre Martínez.

Los archivos `.qmd` contienen el manuscrito. La carpeta `formalization/`
contiene las definiciones y las demostraciones en Lean, junto sus instrucciones
de compilación. 

### Generar el PDF

Se requieren [Quarto](https://quarto.org/), una distribución de LaTeX y la fuente JuliaMono.

Para instalar TinyTeX desde Quarto:

```sh
quarto install tinytex
```

Para generar el documento:

```sh
quarto render
```

Para abrir una vista previa durante la edición:

```sh
quarto preview
```

El PDF generado se guarda en `_book/`. 
